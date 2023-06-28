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
        sh '''hostname;
#curl -sk http://10.60.4.207:7001/console --head;
echo "PROBANDO JENKINS";
date;
df -h .'''
        mail(subject: 'Prueba envio de correo Jenkins pipeline', body: 'Prueba envio de correo Jenkins pipeline', to: 'juliorod@kyndryl.com', from: 'ansibleorbis')
      }
    }

  }
}