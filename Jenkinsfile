pipeline {
   stages {
    stage('Docker node test') {
      agent {
        docker {
          image 'maven:3.3.3'
          args '--name docker-node' // list any args
        }
      }
      steps {
        // Steps run in node:7-alpine docker container on docker slave
        sh 'mvn --version'
      }
    }

    /** stage('Docker maven test') {
      agent {
        docker {
          image 'maven:3-alpine'
        }
      }
      steps {
        // Steps run in maven:3-alpine docker container on docker slave
        sh 'mvn --version'
      }
    }
  }
  
  agent {
    docker {
      image '\'maven:3.3.3\''
    }

  }
  stages {
    stage('build') {
      steps {
        sh '\'mvn --version\''
      }
    } **/

  }
}
