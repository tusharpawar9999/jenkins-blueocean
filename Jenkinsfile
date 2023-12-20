pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
'''
        sh 'date'
        sh '''ls

'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh '''date 
'''
          }
        }

        stage('test par') {
          steps {
            echo 'test parllel'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy 1st '
      }
    }

    stage('production deploy') {
      steps {
        sh 'touch test2223.txt'
        echo 'hello world i am tushar pawar'
      }
    }

  }
}