pipeline {
  agent any
  stages {
    stage("git pull"){
      steps {
        echo "This is git pull stage"
      }
    }
    stage("build"){
      steps {
        echo "This is build stage"
      }
    }
    stage("test"){
      steps { 
        echo "This is test stage"
      }
    }
    stage("artifacts"){
      steps {
        echo "This stage is upload artifacts to JFrog"
      }
    }
  }
  post {
    echo "Any post pipeline steps go here"
  }
}
