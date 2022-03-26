pipeline {
    agent none 
    stages {
        stage('Install Composer') {
            steps {
                sh 'composer install'
            }
        }
        stage('Migration database') { 
            steps {
                sh 'php artisan key:generate'
                sh 'php artisan migrate'
            }
        }
    }
}

