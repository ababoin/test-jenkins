pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'whoami'
                sh 'uname'
                sh 'uname -a'
                sh 'ifconfig'
                sh 'pwd'
                sh 'ls -lah'
                sh 'ls -lah /'
                sh 'ls -lah /etc'
                sh 'ls -lah /var/run'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
