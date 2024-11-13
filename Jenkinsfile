pipeline {
    agent any

    stages {
        stage('Run Parallel Branches') {
            parallel {
                stage('Branch A') {
                    steps {
                        echo "This is branch A"
                    }
                }
                stage('Branch B') {
                    steps {
                        echo "This is branch B"
                    }
                }
            }
        }
    }
}
    
