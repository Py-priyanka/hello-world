pipeline {
    agent {
        node {
            label 'agent1'
        }
    }

environment {
    
    PATH = "/opt/apache-maven-3.9.9/bin:$PATH"
}
    stages {
        stage('clone') {
            steps {
                git 'https://github.com/Py-priyanka/hello-world.git'
            }
        }
        stage('build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}

