pipeline{
    agent 
    docker {image 'jacoblincool/playwright:all'}

    stages{
        stage("verifier la version playwright"){
            stage("install les dependances"){
                sh'npm install'
            }
             steps("verifier la version"){
               sh'npx playwright --version' 
            }
            stage("tester"){
                sh'npx playwright test'
            }
        }
       }
    }
