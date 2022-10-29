pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                sh "ls -la"
                ansiblePlaybook credentialsId: 'ubuntu2', inventory: 'ansible/inventory/test-task/hosts.yml', playbook: 'ansible/nginx.yml'
            }
        }
    }
}
