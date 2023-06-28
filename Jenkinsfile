pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'este el primer paso'
        sh '''echo " esto si que es una prueba"
hostname
who'''
      }
    }

    stage('Estapa2') {
      steps {
        echo 'Este eun paso del la etapa2 de  este pipeline'
      }
    }

    stage('validando openshift sandbox') {
      steps {
        openshiftVerifyService(svcName: 'mongo', namespace: 'k-juliorod-dev', apiURL: 'https://api.sandbox-m4.g2pi.p1.openshiftapps.com:6443', authToken: 'sha256~JlcRprFMsp1krXmu2ELNQR7LsBYEI6kILe9USJA-trE')
      }
    }

  }
}