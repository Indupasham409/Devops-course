pipeline {
    agent any
    triggers {
        pollSCM('* * * * *') // Polls SCM every minute; adjust as necessary
    }
    stages {
        stage('Pull and Deploy') {
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
