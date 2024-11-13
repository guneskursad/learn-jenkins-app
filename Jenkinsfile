pipeline {
    agent any

    stages {
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
