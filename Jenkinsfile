pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        build 'build'
        node(label: 'node') {
          waitForQualityGate(credentialsId: '124801', abortPipeline: true, webhookSecretId: 'Iv1.0de266e2a68ecd5b')
        }

      }
    }

  }
}