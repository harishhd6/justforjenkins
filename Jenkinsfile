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
                    def workspacePath = pwd() // Gets the current workspace directory
                    sh '''
                        echo "This is harikrishna.txt file content" > harikrishna.txt
                        echo "This is vimal.txt file content" > vimal.txt
                    '''
                    // Move the created files to the desired location
                    sh "mv ${workspacePath}/harikrishna.txt /home/ubuntu/harikrishna.txt"
                    sh "mv ${workspacePath}/vimal.txt /home/ubuntu/vimal.txt"
                }
            }
        }
    }
}
