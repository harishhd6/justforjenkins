pipeline {
    agent {
        node {
            name 'slave1'
            label 'jailer'
        }
    }
    stages {
        stage('Create File') {
            steps {
                script {
                    echo "Current User: ${whoami()}"
                    echo "Current Working Directory: ${pwd()}"
                    sh 'env' // Print environment variables
                    sh '''
                        echo "hari is good" > /tmp/proo.txt
                    '''
                }
            }
        }
    }
}
