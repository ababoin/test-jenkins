pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'whoami'
                sh 'uname -a'
                sh 'pwd'
                sh 'ls -lah'
                sh 'ls -lah /'
                sh 'ls -lah /bin'
                sh 'ls -lah /usr'
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
