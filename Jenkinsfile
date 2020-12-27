pipeline {
    agent any
    stages {
        stage ("run server") {
            steps {
                sh './manage.py runserver'
            }
        }
    }
}