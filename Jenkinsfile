pipeline {  
    agent any  
    stages {
        stage('Clone repository') {  
            steps {  
                git clone this repository  
            }
        }
        stage('Build and run docker'){
            steps {
                sudo docker build -t hello-word-php-apache . 
                sudo docker run -p 81:80 hello-word-php-apache
            }
        }
        stage('Prueba página') {
            steps {
                wget http://localhost:81
            }
        }
    }
} 