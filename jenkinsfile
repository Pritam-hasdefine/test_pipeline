pipeline {
    agent any

     stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
               git branch: '*/main', credentialsId: '7cc5f77a-81ae-48c8-8a34-07fc68f71414', url: 'https://github.com/Pritam-hasdefine/apache2.git'
                
                sh 'rsync index.html /var/www/html'
            }
        }
    }
}
