pipeline {
  agent { label 'agent'}
     stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/jeffreydavid/webserverrepo.git'
            }
        }

        stage('Deploy index.html') {
            steps {
                // Assuming the destination is /var/www/html/
                sh 'cp index.html /var/www/html/'
            }
        }
    }
