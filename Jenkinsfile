pipeline {
    agent any
    stages {
        stage('Run Script') {
            steps {
                sh '''
                chmox +x helloWorld.sh
                ./helloWorld.sh Hi
                '''
            }
        }
        stage('Archive Cowsay') {
            steps {
                sh '''
                cowsay "Good Job Class" > wew.txt
                '''
            }
        }
    }
}