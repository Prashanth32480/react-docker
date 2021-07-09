pipeline{
  agent any
  stage{
    stage('Compile stage'){
      steps{
        withMaven(maven : 'maven_'){
          sh 'mvn clean compile'
        }
      }
    }
    stage('Testing stage'){
      steps{
        withMaven(maven : 'maven_'){
          sh 'mvn test'
        }
      }
    }
    stage('Deployment stage'){
      steps{
        withMaven(maveb : 'maven_'){
          sh 'mvn deployment'
        }
      }
    }
  }
}
    
