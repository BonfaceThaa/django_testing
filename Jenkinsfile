pipeline {
    agent any
    stages {
        stage ("env setup ") {
            steps {
                sh 'python3 -m venv testEnv'
                sh 'source testEnv/bin/activate'
                sh 'pip install -r superlists/requirements.txt'
            }
        }
        stage ("run server") {
            steps {
                sh 'python superlists/manage.py runserver'
            }
        }
    }
}