pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        build 'PES2UG21CS382-1'
        sh 'g++ newmain.cpp -o output'
      }
    }
    stage('Test'){
      steps{
        sh './output'
      }
    }
    stage('Deploy'){
      steps{
        echo 'deploy'
      }
    }
  }
  post{
    failure{
      error 'Pipeline failed'
    }
  }
}
