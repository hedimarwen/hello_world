node {
        stage('Poll') {
            checkout scm
        }
        stage('Build') {
            mvn install
        }
        stage('Test') {
            mvn test
        }
        stage('Deploy') {
            mvn deploy
        }
}
