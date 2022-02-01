pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        echo 'Building repository'
        bat 'npm install'
      }
    }
    stage('Scan') {
      steps {
        echo 'Scanning repository'
        bat 'java -jar "C:\\Unified_Agent\\wss-unified-agent.jar" -c "C:\\Unified_Agent\\wss-unified-agent.config" -d "." -product "jenkinsTraining" -project "jenkinsTraining"'
      }
    }
  }
}
