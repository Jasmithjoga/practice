pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                bat 'docker build -t myapp .'
            }
        }
        stage('Deploy'){
            steps{
                bat 'docker run -d -p 5001:5001 myapp'
                // Add deployment commands here
            }
        }
    }
}
