pipeline {
    agent {
        node {
            label 'Deployment'
        }
    }
    stages {
        stage ('COPY') {
            steps {
                sh 'sudo cp -r * /var/www/html'
            }
        }
    }
}
