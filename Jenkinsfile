pipeline {
    agent any
    triggers {
        pollSCM('* * * * *') // Polls SCM every minute; adjust as necessary
    }
    stages {
        stage('Pull and Deploy hi') {
            steps {
                checkout scm
                script {
                    sh '''
                        mkdir -p /path/to/folder
                        cp -R * /path/to/folder
                    '''
                }
            }
        }
    }
}
