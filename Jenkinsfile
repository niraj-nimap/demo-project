pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                python --version
                pip --version 

            }
        }
            }
        }
        stage('Deploy'){
            steps{
                pip install -r requirements.txt --break-system-packages
                python app.py
            }
        }