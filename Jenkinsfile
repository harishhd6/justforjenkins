pipeline {
    agent {
        label 'jailer'
    }
    stages {
        stage('Create File') {
            steps {
                script {
                    // Run the shell command to create the file
                    sh 'touch harikrishna.txt'
                    echo 'harikrishna.txt created successfully!'
                }
            }
        }
    }
    post {
        always {
            // Clean up workspace (optional)
            deleteDir()
        }
    }
}
