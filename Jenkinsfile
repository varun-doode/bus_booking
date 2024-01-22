pipeline {
    agent {
        label 'slave1'
    }

       stages {
        stage('checkout') {
            steps {
                sh 'rm -rf bus_booking'
                sh 'git clone https://github.com/varun-doode/bus_booking.git'
            }
        }

        stage('build') {
            steps {
                script {
                    sh 'mvn --version'
                    sh 'mvn clean install'
                }
            }
        }
        
       
