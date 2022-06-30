pipeline {
    agent {
        node {
            label 'master'
        }
    }

    environment {
        var1 = 'hello'
        var2 = 'how are you'
    }

    tools {
        maven 'maven'
    }

    stages {
        stage('wlecome') {
            steps {
                echo "$var1 Mahendra $var2"
            }
        }
    }

    post {
        success {
            echo "pipeline is successful"
        }

        failure {
            echo "pipeline failed"
        }
    }
}
