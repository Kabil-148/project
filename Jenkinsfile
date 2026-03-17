pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/Kabil-148/project.git'
            }
        }

        stage('Deploy') {
            steps {
                sh 'ansible-playbook -i inventory deploy.yml'
            }
        }
    }
}
