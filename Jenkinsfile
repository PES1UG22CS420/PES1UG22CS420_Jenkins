pipeline {
  agent any
  stages {
    // stage('Clone repository'){
      // steps{
        // checkout([$class: 'GitSCM',
        // branches: [[name: '*/main']],
        // userRemoteConfigs: [[url: 'https://github.com/PES1UG22CS420/PES1UG22CS420_Jenkins.git']])
      // }
    // }
    stage('Build'){
      steps{
        build 'PES1UG22CS420-1'
        sh 'g++ main.cpp -o output'
      }
    }
    stage('Test'){
      steps{
        sh './output'
      }
    }
    stage('Deploy'){
      steps{
        echo 'DISPLAY'
      }
    }
  }
  post{
    failure{
      error: 'Pipeline FAILED!'
    }
  }
}
        
