node {
        stage('Poll') {
            checkout scm
        }
        stage('Build') {
            withMaven(maven:'maven'){
                    bat 'mvn install';
                }
        }
        stage('Test') {
            withMaven(maven:'maven'){
                    bat 'mvn test';
                }
        }
        stage('Deploy') {
            withMaven(maven:'maven'){
                    bat 'mvn deploy';
                }
        }
     }
