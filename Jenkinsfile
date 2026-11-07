pipeline {
    agent any

    stages {
        stage('Create new file') {
            steps {
                script {
                    if (isUnix()) {
                        sh 'touch new_file.txt'
                    } else {
                        bat 'type nul > new_file.txt'
                    }
                }
            }
        }

        stage('Print Message') {
            steps {
                echo 'Hello from Pipeline!'
            }
        }
    }
}

