pipeline{
    agent {
    docker {image 'mcr.microsoft.com/playwright:v1.50.0-noble'}
    }
}
stages{
        stage("install les dependence"){
            steps{
                sh'npm install'
            }
        }
        stage("verfier la version"){
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
    