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
    stage(run e2e) {
      when {
        expression {
          BRANCH_NAME = "DEV"
        }
      }
      steps {
        ehco "Running e2e tests in headless environment."
      }
    }
    stage("artifacts"){
      steps {
        echo "This stage is upload artifacts to JFrog"
      }
    }
  }
  post {
    always {
      echo "Post build steps go here!"
    }
  }
}
