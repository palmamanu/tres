pipeline {
    stages {
     parallel {
        stage('Build') {
            echo 'Building...'
         }
        
        stage('estadoparalelo') {
          steps {
            echo 'empieza el estado'
            ansiblePlaybook(installation: 'ansible', playbook: '/tmp/apache.yml')
            pwd(tmp: true)
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
