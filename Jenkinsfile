pipeline {
    agent any

    stages {
        stage('dev') {
            steps {
                echo 'Hello World -dev'
            }
        }
      stage('qa') {
            steps {
                echo 'Hello World - qa'
            }
        }
      stage('prod') {
            steps {
                echo 'Hello World - prod'
            }
        }
    }
    post {
        always {
            echo 'Always build executed'
        }
        success {
            echo 'success build executed'

        }
        failure {
            echo 'failure build executed'
        }
    }
}
