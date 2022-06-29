CODE_CHANGES = getGitChanges()
pipeline {
    agent any

    stages {
        stage('dev') {
            when {
                expression {
                    BRANCH_NAME = 'main' && CODE_CHANGES == true
                }
            }
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
