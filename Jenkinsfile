pipeline {
    agent any

    stages {
        stage('Pull Code') {
            steps {
                // Clean workspace before pulling the code (optional)
                deleteDir()

                // Clone the Git repository
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/Sayan6726/demo-html.git'
            }
        }

        stage('Copy Project'){
            steps{
                sh 'cp -rf . /var/www/html/demo-html'
            }
        }

    }
}

