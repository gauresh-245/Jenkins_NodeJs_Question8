pipeline {
    agent any

    stages {
        stage('Fetch File from my repo') {
            steps {
                git branch: 'main', url: 'https://github.com/gauresh-245/Jenkins_NodeJs_Question8.git'
            }
            
        }
        stage('build my file'){
            steps {
                echo 'Build Project'
                bat 'javac print.java'
               
            }
        }
        stage('Execute'){
            steps {
                echo 'Executingg'
                bat 'java print'
            }
        }
        stage('Deploy'){
            steps {
                echo 'Deploying'
               
            }
        }
    }
    post{
        success{
            echo 'pipeline successful'
        }
        failure{
            echo 'pipeline failed'
        }
    }
}
