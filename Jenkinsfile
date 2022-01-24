pipeline {  
    agent any  
    stages {
        stage('Clone repository') {  
            steps {  
                git clone this repository  
            }
        }
        stage('Build docker'){
            steps {
                sudo docker build -t hello-word-php-apache . 
            }
        }
        stage('Run docker') {
            steps {
                sudo docker run -p 81:80 hello-word-php-apache
            }
        }
    }
} 
