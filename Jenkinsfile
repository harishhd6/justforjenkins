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
                    // Create harikrishna.txt file
                    sh 'echo "Hello, Harikrishna!" > harikrishna.txt'
                    
                    // Create vimal.txt file
                    sh 'echo "Hello, Vimal!" > vimal.txt'
                    sh 'echo "Hello, Vimal!" > vi.txt'
                    
                    // Verify files are created
                    sh 'ls -l'
                }
            }
        }
    }
}
