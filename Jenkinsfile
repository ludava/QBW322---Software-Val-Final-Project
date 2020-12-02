pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn -B -DskipTests clean package'
      }
    }

    stage('Test') {
      steps {
        sh 'mvn test'
        echo 'This is the first test case - QBW___'
        echo 'Test 2  - QBW___'
      }
    }

    stage('Deliver') {
      steps {
        echo 'Reached Delivery - QBW___'
      }
    }

  }
}