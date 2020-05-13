pipeline {
  agent any
  stages {
    stage('Pull') {
      steps {
        echo 'Pullen van Git'
        git 'https://github.com/NickSoons/2TIN_ResearchProject.git'
      }
    }

    stage('build') {
      steps {
        echo 'Builden'
      }
    }

    stage('Test') {
      steps {
        echo 'Testen'
      }
    }

    stage('Artifact') {
      steps {
        echo 'Artifact aanmaken'
        archiveArtifacts(allowEmptyArchive: true, artifacts: '/tmp/bla')
      }
    }

    stage('Deployment') {
      steps {
        echo 'Deployment naar de webserver'
      }
    }

  }
}