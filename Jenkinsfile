pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat(script: 'mvn -B -DskipTests clean package', encoding: 'UTF-8')
      }
    }

    stage('Test') {
      steps {
        echo 'This is the first test case - QBW___'
        echo 'Test 2  - QBW___'
        bat(script: 'mvn test', encoding: 'UTF-8')
      }
    }

    stage('Deliver') {
      steps {
        echo 'Reached Delivery - QBW___'
      }
    }

  }
}