pipeline {
  agent any
  stages {
    stage("git pull"){
      echo "This is git pull stage"
    }
    stage("build"){
      echo "This is build stage"
    }
    stage("test"){
      echo "This is test stage"
    }
    stage("artifacts"){
      echo "This stage is upload artifacts to JFrog"
    }
  }
  post {
    echo "Any post pipeline steps go here"
  }
}
