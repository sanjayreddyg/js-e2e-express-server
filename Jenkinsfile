pipeline {
    agent { label 'JDK11' }
    stages{
        stage('Source Code') {
            steps {
                git url: https://github.com/sanjayreddyg/js-e2e-express-server.git,
                branch: 'main'
            }
          stage('install dependancies') {
              
            steps{
                
                sh 'npm install'
            }
        }
        stage('npm build') {
            
            steps {
                
                sh 'npm run build'
            }
        }
        
        }