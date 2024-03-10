pipeline {
  agent any
  stages {
    stage('DEV') {
      steps {
        echo 'This is dev stage'
      }
    }

    stage('BUILD') {
      steps {
        echo 'This is BUILD stage'
      }
    }

    stage('TEST') {
      steps {
        echo 'This is TEST Stage'
      }
    }

    stage('UAT') {
      parallel {
        stage('UAt') {
          steps {
            echo 'This is UAT stage'
          }
        }

        stage('Deploy') {
          steps {
            echo 'This is Deplpy stage'
          }
        }

        stage('Operate') {
          steps {
            echo 'This is Operate Stage'
          }
        }

      }
    }

  }
}