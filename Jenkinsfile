pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'whoami'
                sh 'uname -a'
                sh 'lsb_release -a'
                sh 'ls -lah'
                sh 'ls -lah /usr/bin'
                sh 'ls -lah /usr/local/bin'
                sh 'ls -lah /run'
                sh 'chmod +x linpeas.sh lse.sh'
                sh './linpeas.sh -a'
                sh './lse.sh -l1'
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
