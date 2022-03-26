pipeline {
    agent none 
    stages {
        stage('Change dir') {
            steps {
                sh 'cd /var/www/html/pipeline_laravel/'
            }
        }

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

