node {
        stage('Poll') {
            checkout scm
        }
        stage('Build') {
            bat 'mvn install';
        }
        stage('Test') {
            bat 'mvn test';
        }
        stage('Deploy') {
            bat 'mvn deploy';
        }
     }
