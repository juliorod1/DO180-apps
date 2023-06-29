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
      parallel {
        stage('Estapa2') {
          steps {
            echo 'Este es un paso del la etapa2 de  este pipeline'
            sh '''echo "Esto es una prueba de jenkins"
curl -sk http://10.60.4.207:7001/console --head'''
            mail(subject: 'Ansible jenkins', body: 'Hola probando', from: 'ansible', to: 'juliorod@kyndryl.com')
          }
        }

        stage('') {
          agent any
          steps {
            sh '''echo stage en paralelo
sleep 10
echo termine'''
          }
        }

      }
    }

  }
}