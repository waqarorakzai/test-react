pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                script {
                   def tools = tool 'NodeJs21'
                    echo "Node.js Home: ${tools}"
                    sh "${tools}/bin/node --version"
                    sh "${tools}/bin/npm --version"
                }
            }
        }
    }
}
