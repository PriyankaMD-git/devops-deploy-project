pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/PriyankaMD-git/devops-deploy-project.git'
            }
        }

        stage('Run Ansible Playbook') {
            steps {
                sh 'ansible-playbook -i inventory playbook.yml'
            }
        }
    }
}
