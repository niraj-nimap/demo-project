pipeline {

    agent any

    stages {

        stage('Build') {
            steps {
                sh "python --version && pip --version"
            }
        }

        stage('Deploy') {
            steps {
                sh "pip install -r requirements.txt --break-system-packages"

                sh "nohup python app.py > output.log 2>&1 &"
            }
        }
    }
}