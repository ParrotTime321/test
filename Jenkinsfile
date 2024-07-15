pipeline {
    agent any

    environment {
        WORKSPACE = "/home/ubuntu/"
    }

    stages {
        stage('Who am i and pwd') { 
            steps {
                sh 'whoami'
                sh 'pwd'
            }
        }
        stage('Hello') { 
            steps {
                dir("${WORKSPACE}") {
                    sh 'mkdir -p home/ubuntu'
                    sh 'cd home/ubuntu'
                    echo 'Hello World 2'
                    sh 'whoami'
                    sh 'pwd'
                }
            }
        }
        stage('Shell1') {
            steps {
                sh 'echo "Listing /etc/netplan:"'
                sh 'ls -l /etc/netplan'
            }
        }
        stage('Shell2') {
            steps {
                sh 'echo "Listing /home:"'
                sh 'ls -l /home/'
            }
        }
    }
}
