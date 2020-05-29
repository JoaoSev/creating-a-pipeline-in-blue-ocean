pipeline {
  agent any
  stages {
    stage('Build Solution') {
      parallel {
        stage('Minimum Version') {
          steps {
            echo 'Minimum Version'
          }
        }

        stage('Latest Main Release') {
          steps {
            echo 'Latest Main Release'
          }
        }

        stage('Latest Feature Release') {
          steps {
            echo 'Latest Feature Release'
          }
        }

      }
    }

    stage('Build Package') {
      steps {
        echo 'Build Application Install Package'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy Package to SVN'
      }
    }

  }
}