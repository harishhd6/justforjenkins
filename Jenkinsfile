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
                    sh '''
                        echo "This is harikrishna.txt file content" > /home/ubuntu/harikrishna.txt
                        echo "This is vimal.txt file content" > /home/ubuntu/vimal.txt
                    '''
                }
            }
        }
    }
}
