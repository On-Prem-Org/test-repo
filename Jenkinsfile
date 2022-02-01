pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        echo 'Building repository'
        npm install
      }
    }
    stage('Scan') {
      steps {
        echo 'Scanning repository'
        java -jar C:\\Unified_Agent\\wss-unified-agent.jar -d .
      }
    }
  }
}
