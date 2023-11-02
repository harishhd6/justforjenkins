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
                        echo "hari is good" > /var/tmp/proo.txt
                    '''
                }
            }
        }
    }
}
