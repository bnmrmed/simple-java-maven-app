pipeline {
        agent {
            label 'docker-gce'
            image 'agilefabric-docker-virtual.enterpriserepo.fr.carrefour.com/maven:3-jdk-11' 
            args '-v /root/.m2:/root/.m2' 
        }
    stages {
        stage('Build') { 
            steps {
                sh 'echo hello' 
            }
        }
    }
}
