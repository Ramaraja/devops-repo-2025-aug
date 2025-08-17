pipeline {
    agent { docker { image 'python:3.12.0-alpine3.18' } }
    stages {
        stage('Setting up env') {
            steps {
                    sh 'python3 -m venv venv'
                    sh '. venv/bin/activate && pip install -r sample-project-1/requirements.txt'      
            }
        }
    }
}
