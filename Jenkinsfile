pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                script {
                   ef tools = tool 'NodeJs21'
                    def nodeBin = "${tools}/bin/node"
                    def npmBin = "${tools}/bin/npm"
                    echo "Node.js Home: ${tools}"
                    sh "${nodeBin} --version"
                    sh "${npmBin} --version"
                }
            }
        }
    }
}
