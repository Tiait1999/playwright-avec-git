pipeline{
    agent 
    docker {image 'mcr.microsoft.com/playwright:v1.50.0-noble'}

    stages{
        stage("verifier la version playwright"){
            steps("install les dependances"){
                sh'npm install'
            }
             stage("verifier la version"){
                steps{
                     sh'npx playwright --version' 
                }
            }
            stage("tester"){
                steps{
                    sh'npx playwright test'
                }
                
            }
        }
       }
    }
