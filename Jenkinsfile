pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/ArjunDivraniya/Jenkins-Test.git'
            }
        }

        stage('Run Java') {
            steps {
                sh '''
                echo "Running Java Program"
                javac Main.java
                java Main
                '''
            }
        }

        stage('Run Node') {
            steps {
                sh '''
                echo "Running Node Program"
                node index.js
                '''
            }
        }
    }
}