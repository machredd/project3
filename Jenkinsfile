pipeline
{
agent any

  tools{

maven 'M3'
jdk 'JAVA_HOME'
  }
  stages{
stage('Checkout'){
  steps{
git branch: 'master',url:'https://github.com/machredd/project3.git'
  }
}
    stage('Build'){
steps{
bat 'mvn compile'
}
    }
    stage ('Package'){
steps
      {
bat 'mvn package'
      }
    }
    
    stage('Deploy'){
      steps{
bat 'Java -jar C:/Program Files/Jenkins/workspace/ecommercebeckend/target/ecommercebackend-0.0.1-SHAPSHOT.jar'
      }
    }
  }
}
