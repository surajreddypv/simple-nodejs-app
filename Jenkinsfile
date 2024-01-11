pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'npm install express --save'
                // sh 'npm install -g pm2'
            }
        }
        stage('deploy') {
            steps {
                sh 'npm start'
                sh 'node index.js &'
                // sh 'pm2 start index.js'
                sh 'npm stop'
            }
        }
        
    }
}
