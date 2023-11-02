pipeline {
    agent {
        node('jailer') {
            label 'jailer'
        }
    }
    stages {
        stage('Create Files') {
            steps {
                script {
                    // Create harikrishna.txt file in /home/ubuntu directory
                    sh 'echo "Hello, Harikrishna!" > /home/ubuntu/harikrishna.txt'
                    
                    // Create vimal.txt file in /home/ubuntu directory
                    sh 'echo "Hello, Vimal!" > /home/ubuntu/vimal.txt'
                    
                    // Verify files are created
                    sh 'ls -l /home/ubuntu'
                }
            }
        }
    }
}
