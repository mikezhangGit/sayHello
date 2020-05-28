pipeline {
  agent any
  
  stages {
    build "say-Talk"
    
    stage('sayHello') {
      parallel {
        stage('callWinBat') {
          steps {
            bat(script: 'echo "--- hello,  mike ..."', returnStdout: true)
          }
        }

        stage('callUnixSh') {
          steps {
            sh 'echo "--- this is a shell to run for test ..."'
          }
        }

      }
    }
    
    

  }
}
