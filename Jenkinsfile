pipeline {
    agent any
    stages {
        stage('---clean---') {
            steps {
                sh "mvn clean"
            }
        }
        stage('--test--') {
            steps {
                sh "mvn test"
            }
        }
        stage('--package--') {
            steps {
                sh "mvn package"
            }
        }
        stage('--run--'){
            steps{
                sh 'java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App'
            }
        }
    }
}