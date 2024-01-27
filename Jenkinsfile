pipeline {
  agent any
  stages {
    stage("git pull"){
      step {
        echo "This is git pull stage"
      }
    }
    stage("build"){
      step {
        echo "This is build stage"
      }
    }
    stage("test"){
      step{ 
        echo "This is test stage"
      }
    }
    stage("artifacts"){
      step{
        echo "This stage is upload artifacts to JFrog"
      }
    }
  }
  post {
    echo "Any post pipeline steps go here"
  }
}
