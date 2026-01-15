pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // This clones the repository to the Jenkins workspace
                git url: 'https://github.com/thegame-ali/spring-jenkins.git', branch: 'main'
            }
        }
        
        stage('Print Message') {
            steps {
                // This prints to the Jenkins Console Output
                echo 'Successfully connected to the spring-jenkins repository!'
                
                // You can also run shell commands to list files or print system info
                sh 'ls -ltr'
                sh 'echo "Current workspace directory is: $(pwd)"'
            }
        }
    }
}


