pipeline {
  agent any
  stages {
    stage('sayHello') {
      parallel {
        stage('callWinBat') {
          steps {
            bat(script: 'echo "--- hello,  mike ..."', returnStdout: true)
          }
        }

        stage('error') {
          steps {
            sh 'echo "--- this is a shell to run for test ..."'
          }
        }

      }
    }

  }
}