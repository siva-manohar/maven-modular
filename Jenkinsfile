pipeline {

    tools {
        maven "maven"
        java "jdk17"
    }

    stages {

        stage('intialize') {
            steps {
                echo "PATH=${MAVEN_HOME}/bin:{$PATH}"
                echo "MAVEN_HOME=/home/ubuntu/apache-maven-3.8.8"
            }
        }

        stage('build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}