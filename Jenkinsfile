pipeline {
    agent {label "nginx_tst2"}
    stages {
        stage("Checkout") {
            steps {
                git 'https://github.com/andy-dkit/devops-ex1.git'
                echo "Stage 1- Checkout"
                sh "pwd"
            }
        }
        stage("Copy Files to Nginx") {
            sh "cp * /usr/share/nginx/html"
        }       
    }
}
