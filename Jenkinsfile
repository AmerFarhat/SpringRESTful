pipeline{
  agent any
  tools {maven "Amer"}
  stages{
    stage("checkout"){
      steps{
        git branch: "main", url: "https://github.com/AmerFarhat/SpringRESTful.git"
      }
      
    }
    stage("build"){
      steps{
        sh "mvn compile"
      }
    }
    stage("test"){
      steps{
        sh "mvn test"
      }
    }
  }
}
