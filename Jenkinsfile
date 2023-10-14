pipeline {
    agent any // Use 'any' agent type to run the pipeline on any available agent

    stages {
        stage('Build') {
            steps {
                script {
                    // Run the pipeline inside a Docker container
                    docker.image('node:16').inside {
                        // Inside the Docker container, run the npm install command
                        sh 'npm install --save'
                    }
                }
            }
        }
    }
}
