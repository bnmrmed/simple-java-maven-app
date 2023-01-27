pipeline {
      agent {
        docker {
          image 'maven:3-jdk-11'
          registryUrl 'https://agilefabric-docker-virtual.enterpriserepo.fr.carrefour.com/'
          //registryCredentialsId 'af_private_registry_sa'
          label 'docker-gce'
          //reuseNode true
        }
    stages {
        stage('Build') { 
            steps {
                sh 'echo ls '
                sh 'pwd'
                sh 'ls'
            }
        }
    }
}
