pipeline {
    agent any
    stages {
         stage('helloworld') {
            when {
                branch 'hello'
            }
            steps {
                sh 'npm install express --save'
                 // sh 'npm install -g pm2'
                sh 'npm start'
                sh 'node index.js'
                // sh 'pm2 start index.js'
            }
        }
        stage('simple_node_app') {
            when {
                branch 'master'
            }
            steps {
                sh 'npm install express --save'
                 // sh 'npm install -g pm2'
                sh 'npm start'
                sh 'node app.js'
            }
        }

    }

}
