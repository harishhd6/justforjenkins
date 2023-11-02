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
                    sh '''
                        echo "hari is good" > /home/ubuntu/proo.txt
                    '''
                }
            }
        }
    }
}
