pipeline {
    agent {lable:'mynode001'}

    stages {
        stage('Hello') {
            steps {
                echo 'Hi'
                echo 'Hello'
                echo 'World'
                echo 'this is maha'
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
