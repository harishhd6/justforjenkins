pipeline {
    agent {
        node {
            name 'slave1'
            label 'jailer'
        }
    }
    stages {
        stage('Create Files') {
            steps {
                script {
                    echo "Current Working Directory: ${pwd()}"
                    echo "User: ${whoami()}"
                    sh 'env' // Print environment variables
                    sh '''
                        echo "This is harikrishna.txt file content" > harikrishna.txt
                        echo "This is vimal.txt file content" > vimal.txt
                    '''
                    sh 'ls -l' // List files in the current directory for debugging
                    // Move the created files to the desired location
                    sh "mv harikrishna.txt /home/ubuntu/harikrishna.txt"
                    sh "mv vimal.txt /home/ubuntu/vimal.txt"
                }
            }
        }
    }
}
