pipeline {
    agent any

    environment {
        // Set the Node.js version, adjust as needed
        NODEJS_VERSION = '19.9.0'
    }

    stages {
        stage('Install Dependencies') {
            steps {
                script {
                    // Use nvm to install the specified Node.js version
                    def npmHome = tool name: "NodeJS ${NODEJS_VERSION}", type: 'npm'
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
