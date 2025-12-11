pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('clone java project') {
            steps {
               git 'https://github.com/maha4dsvc/mahalogin.git'
            }
        }
        
         stage('execute maven target') {
            steps {
             sh 'mvn clean install'
            }
        }
    }
}
