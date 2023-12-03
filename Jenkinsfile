pipeline {
  agent any
  tools {
    maven 'Maven'
  }
  stages {
    stage ('Initialize') {
      steps {
        sh '''
                      echo "PATH = ${PATH}"
                      ECHO "M2_HOME = ${M2_HOME}"
           '''
      } 
    }
    stage ('Build') {
      steps {
      sh 'mvm clean package'
    }
    }
    
  }
}
