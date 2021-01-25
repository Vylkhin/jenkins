pipeline {
    agent { 
      docker {
        image 'hashicorp/terraform'
        args  '--entrypoint='
      }
    }
    stages {
        stage('Launch') {
            steps {
                sh 'python /srv/test/test.py'
            }
        }
        stage('Echo') {
            steps {
                sh 'whoami'
            }
        }
    }
}
