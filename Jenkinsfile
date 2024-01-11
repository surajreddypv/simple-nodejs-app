pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'npm install express --save'
            }
        }
        stage('deploy') {
            steps {
                sh 'npm start'
                // sh 'node index.js &'
                sh 'pm2 start index.js'
                // sh 'npm stop'
            }
        }
        
    }
}
