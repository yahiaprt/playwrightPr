pipline {
    agent {
        docker {
            image 'mcr.microsoft.com/playwright:v1.59.1-noble'
            args '-u root --entrypoint='
        }

        paramatres {
        booleanParam(name: 'default_execution_for_all', defaultValue: false, description: 'Run all collections/envs')
        booleanParam(name: 'chose_nav', defaultValue: false, description: 'Run all collections/envs')
                booleanParam(name: 'chose_Tag_option', defaultValue: false, description: 'Run all collections/envs')

        choice(name: 'nav', choices: ['chromium', 'firefox', 'webkit'], description: 'Pick nav')

        }

        stages {
               stage ('test play '){
               steps {
                  sh 'npm install'
               }
            }

            stage ('test play '){
               steps {
                 script {
                          if(chose_nav === true) {
 
                                    sh 'npx playwright test --project = ' ${choice.nav}
                    
        }  else {
                        sh 'npx playwright test'

        }

        if(chose_Tag_option === true && chose_nav === true ){
            sh 'npx playwright --grep "@TNR" --project=' ${nav}
        } else {
            sh 'npx playwright --grep "@TNR" '
        }
            
        


                 }


               }


            }

        }
    }
}