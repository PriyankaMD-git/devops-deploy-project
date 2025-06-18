pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/<your-username>/<your-repo>.git'
            }
        }

        stage('Run Ansible Playbook') {
            steps {
                sh 'ansible-playbook -i inventory playbook.yml'
            }
        }
    }
}
