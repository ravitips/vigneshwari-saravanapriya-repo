pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh """
                    sudo echo "This is my page -version 3" > /var/www/html/index.nginx-debian.html
                 """
            }
        }
        stage('Deploy'){
            steps{
                sh """
                    sudo systemctl restart nginx
                """
            }
        }

    }
}
