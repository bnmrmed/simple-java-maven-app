pipeline {
      agent {
        docker {
          image 'maven:3-jdk-11'
          registryUrl 'https://agilefabric-docker-virtual.enterpriserepo.fr.carrefour.com/'
          label 'docker-gce'
          args '-e MAVEN_OPTS="-Duser.home=/datas" -v /datas:/datas'
        }
      }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests install'
            }
        }
    }
}
