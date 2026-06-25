pipeline{
    agent any
    parameters{
        booleanParam(name:'ALLURE', defaultValue: false, description: 'generation de rapport allure')
        booleanParam(name: 'istags', defaultValue: false, description: 'executer avec ou sans tags')
        choice(name: 'Tags', choices: ['@e2e', '@invalide', '@valide'], description: 'Choisissez le choix de tag')
        booleanParam(name: 'isbrowser', defaultValue: false, description: 'executer avec ou sans browser')
        choice(name: 'browser', choices: ['firefox','chromium','webkit'], description: 'Choisissez le choix du navigateur')   
    }
    stages{
        stage('global stage'){
            agent{
                docker{
                    image 'mcr.microsoft.com/playwright:v1.59.1-noble'
                    args '-u root --entrypoint='
                }
            }
            stages{
                stage('install deps'){
                    steps{
                        sh 'npm ci'
                    }
                }

                stage('clean allure results'){
                    
                    steps{
                        sh '''
                            echo "Suppression du cache Allure..."
                            rm -rf allure-results
                            mkdir -p allure-results
                            echo "Dossier allure-results nettoyé avec succès"
                        '''
                    }
                }
        
                stage('run user test'){
                    steps{  
                        script{
                            if(params.ALLURE){
                                if(params.istags && params.isbrowser){
                                    sh"npx playwright test --grep ${params.Tags} --project=${params.browser} --reporter=allure-playwright"
                                } else if(params.isbrowser){
                                    sh"npx playwright test --project=${params.browser} --reporter=allure-playwright"
                                }else if(params.istags){
                                    sh"npx playwright test --grep ${params.Tags} --reporter=allure-playwright"
                                }else {
                                    sh"npx playwright test --reporter=allure-playwright"
                                }
                                stash name: 'allure-results', includes: 'allure-results/*'
                            }else {
                                if(params.istags && params.isbrowser){
                                    sh"npx playwright test --grep ${params.Tags} --project=${params.browser}"
                                } else if(params.isbrowser){
                                    sh"npx playwright test --project=${params.browser}"
                                }else if(params.istags){
                                    sh"npx playwright test --grep ${params.Tags}"
                                }else {
                                    sh"npx playwright test"
                                }   
                            }
                        }
                    }
                }
            }
        }
    }
    post{
        always{
            script{
                if(params.ALLURE){
                    unstash 'allure-results'
                    archiveArtifacts 'allure-results/*'
                    allure includeProperties: false,
                           jdk: '',
                           results: [[path: 'allure-results/']]
                }
            }
        }
    }
}
 

/*
pipeline {
    agent {
        docker {
            image 'mcr.microsoft.com/playwright:v1.61.0-noble'
            args '-u root --entrypoint='
        }
    }

    parameters {
        booleanParam(name: 'chose_nav', defaultValue: false, description: 'Choose specific browser')
        booleanParam(name: 'chose_Tag_option', defaultValue: false, description: 'Run with @TNR tag')

        choice(name: 'nav', choices: ['chromium', 'firefox', 'webkit'], description: 'Pick browser')
        choice(name: 'tagList', choices: ['@TNR', '@smoke'], description: 'Pick tag')

    }

    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run Playwright Tests') {
            steps {
                script {
                    if (params.chose_nav) {
                        if (params.chose_Tag_option) {
                            sh "npx playwright test --grep" +  ${params.tagList}  + " --project=" + ${params.nav}
                        } else {
                            sh "npx playwright test --project=${params.nav}"
                        }
                    } else {
                        if (params.chose_Tag_option) {
                            sh "npx playwright test --grep" +  ${params.tagList}
                        } else {
                            sh 'npx playwright test'
                        }
                    }
                }
            }
        }
    }
}
*/