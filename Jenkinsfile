pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                script {
                   def tools = tool 'NodeJs21'
                    sh "ls -la ${tools}"
                }
            }
        }
    }
}
