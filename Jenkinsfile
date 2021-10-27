pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'whoami'
                sh 'uname -a'
                sh 'ip addr'
                sh 'pwd'
                sh 'ls -lah'
                sh 'ls -lah /'
                sh 'ls -lah /etc'
                sh 'cat /etc/sudoers'
                sh 'cat /etc/sudo.conf'
                sh 'cat /etc/passwd'
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
