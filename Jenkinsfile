pipeline{
    agent 
    docker {image 'mcr.microsoft.com/playwright:v1.50.0-noble'}

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
