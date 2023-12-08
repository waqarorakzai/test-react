pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                script {
                   def npmHome = tool name: 'NodeJs21', type: 'npm'
                    env.PATH = "${npmHome}/bin:${env.PATH}"
                    sh 'npm install'
                }
            }
        }

        stage('Build') {
            steps {
                script {
                    // Build the React app
                    sh 'npm run build'
                }
            }
        }
    }
}
