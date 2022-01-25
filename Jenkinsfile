pipeline {  
    agent any  
    stages {
        stage('Build and run docker'){
            steps {
                sh "docker build -t hello-word-php-apache ." 
                sh "docker run -p 81:80 hello-word-php-apache -d"
            }
        }
        stage('Prueba página') {
            steps {
                sh "wget http://localhost:81"
            }
        }
    }
} 