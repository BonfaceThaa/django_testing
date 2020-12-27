pipeline {
    agent any
    stages {
        stage ("env setup ") {
            steps {
                withPythonEnv ("~/envs/djangoTestEnv/bin/python3") {
                    pysh 'pip install -r superlists/requirements.txt'
                }
            }
        }
        stage ("run server") {
            steps {
                sh 'python superlists/manage.py runserver'
            }
        }
    }
}