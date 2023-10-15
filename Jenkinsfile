pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {
                script {                   
                    docker.image('node:16').inside {                        
                        sh 'npm install --save'
                    }
                }
            }
        }
    }
}
