pipeline { 
  agent any
  
  environment {
    PROJECT_NAME = "API test"
    OWNER_NAME = "Itay"
  }
  
  stages {
    stage('1=Build') {
      steps {
        echo "Start Stage Build"
        sh 'mvn -version'
      }
    }
  
  }
}
