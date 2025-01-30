pipeline{
  agent any

  
  tools {
    nodejs 'nodejs'
  }

  stages{
   stage('Git Checkout') {
            steps {
                git url: "${env.GIT_URL}", branch: 'master'
            }
        }



   stage('NPM Install') {
            steps {
               sh "npm install"
            }
        }



  stage('Node build') {
            steps {
               sh "npm run build"
            }
        }
    }

    
  }

