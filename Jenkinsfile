pipeline {
    agent any

    stages {
        stage('svn checkout') {
            steps {
                git "https://github.com/naturenaga/sampleproject.git"
            }
        }
        stage('compile package') {
            steps {
                tool name: 'maven-3', type: 'maven'
                sh 'mvn package'
            }
        }
    }
}
