pipeline {
    agent {
        docker {
            image 'mcr.microsoft.com/playwright:v1.59.1-noble'
            args '-u root --entrypoint='
        }
    }

    parameters {
        booleanParam(name: 'chose_nav', defaultValue: false, description: 'Choose specific browser')
        booleanParam(name: 'chose_Tag_option', defaultValue: false, description: 'Run with @TNR tag')

        choice(name: 'nav', choices: ['chromium', 'firefox', 'webkit'], description: 'Pick browser')
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
                            sh "npx playwright test --grep '@TNR' --project=${params.nav}"
                        } else {
                            sh "npx playwright test --project=${params.nav}"
                        }
                    } else {
                        if (params.chose_Tag_option) {
                            sh "npx playwright test --grep '@TNR'"
                        } else {
                            sh 'npx playwright test'
                        }
                    }
                }
            }
        }
    }
}