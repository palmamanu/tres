pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Building...'
            sh 'npm install'
            task 'tarea1'
            pwd(tmp: true)
          }
        }
        stage('prueba2') {
          steps {
            echo 'hola'
            sh '/usr/bin/ansible-playbooks /tmp/apache.yml'
          }
        }
      }
    }
    stage('Test') {
      steps {
        echo 'Testing...'
      }
    }
    stage('Testeadoya') {
      steps {
        echo 'Testing...'
      }
    }
  }
}