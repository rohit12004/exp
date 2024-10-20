pipeline {
  agent any

  stages{

    stage('Build'){
      steps{
      bat 'javac Test.java'
    }
  }
  stage('Run'){
    steps{
      bat 'java Test'
    }
  }
}
}
