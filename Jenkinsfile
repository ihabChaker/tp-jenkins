pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'gradle build'
      }
    }

    stage('Mail') {
      steps {
        mail(subject: 'New Build', body: 'A new build is being published', cc: 'hi_benakcha@esi.dz', from: 'hi_benakcha@esi.dz', to: 'hi_benakcha@esi.dz')
      }
    }

  }
}