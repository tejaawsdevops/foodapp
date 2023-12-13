pipeline {
    agent {
        node {
            label 'Deployment'
        }
    }
    stages {
        stage ('SCM') {
            steps {
                git credentialsId: 'GitHub_ID', url: 'https://github.com/Iftequar7/food.git'
            }
        }
        stage ('COPY') {
            steps {
                sh 'sudo cp -r * /var/www/html'
            }
        }
    }
}
