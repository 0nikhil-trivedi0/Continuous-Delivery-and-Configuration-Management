pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Add build steps here
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Add test steps here
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                ansiblePlaybook(
                    playbook: 'playbook.yml',
                    inventory: 'inventory.ini'
                )
            }
        }
    }
}
