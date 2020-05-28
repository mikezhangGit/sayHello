pipeline {
  agent any
  stages {
    stage('sayHello') {
      parallel {
        stage('sayHello') {
          steps {
            bat(script: 'echo "--- hello,  mike ..."', returnStdout: true)
          }
        }

        stage('') {
          steps {
            sh 'echo "--- this is a shell to run for test ..."'
          }
        }

      }
    }

  }
}