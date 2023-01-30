pipeline {
      agent {
        docker {
          image 'maven:3-jdk-11'
          registryUrl 'https://agilefabric-docker-virtual.enterpriserepo.fr.carrefour.com/'
          //registryCredentialsId 'af_private_registry_sa'
          label 'docker-gce'
          args '-e MAVEN_OPTS="-Duser.home=/datas" -v /datas:/datas'
          //reuseNode true
        }
      }
    stages {
        stage('Build') { 
            steps {
                sh 'echo pwd '
                sh 'pwd'
                sh 'echo ls '
                sh 'ls -al /datas' 
                sh 'mvn -B -DskipTests package'
                sh 'ls -al /datas'
            }
        }
    }
}
