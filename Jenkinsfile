pipeline{
    agent 
    docker { image 'jacoblincool/playwright :latest'}

    stages{
        stage("verifier la version playwright"){
            steps{
               sh'npx playwright --version' 
            }
            stage("install les dependances"){
                sh'npm install'
            }
            stage("tester"){
                sh'npx playwright test'
            }
        }
       }
    }
