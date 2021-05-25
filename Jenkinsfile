@Library('jenkins_shared_library')_ 

BRANCH_NAME = 'master'
GITHUB_CREDENTIALS_ID = 'e63b99a7-0ae5-411b-82af-0e4a4f96b44f'
GIT_REPO = 'https://github.com/igurwitz/karateapitest'

pipeline { 
  agent any
  
  environment {
    PROJECT_NAME = "API test"
    OWNER_NAME = "Itay"
  }
  
  stages {
    stage ('qa-api-automation - Checkout'){
            steps {
                script {
                    
                 	 git branch: BRANCH_NAME, credentialsId: GITHUB_CREDENTIALS_ID, url: GIT_REPO

                    }
                }
            }
   stage('1=Build') {
      steps {
        echo "Start Stage Build"
        sh 'mvn -version'
      }
    }
  
  }
}
