pipeline {
    agent {
        agent {label 'docker-gce'}
    }
    stages {
        stage('Build') { 
            steps {
                sh 'echo hello' 
            }
        }
    }
}
