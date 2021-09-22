    pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git 'https://github.com/Oleg1996Novitsky/django-helloworld.git'
                sh "docker build -t localhost:8080/${BUILD_NUMBER} ."
                sh 'docker-compose up -d'
            }
        }
    }
}
