pipeline {
    agent any
    stage ('run parallel branches') {
            parallel {
              stage ('branch A') {
                echo "This is branch a"
              },
              stage ('branch B') {
                echo "This is branch b"
              }
            }
    }
/*
    stages {
        stage('Build') {
            agent {
                docker {
                    image 'node:18-alpine'
                    reuseNode true
                }
            }
            steps {
                sh '''
                    npm ci
                    npm run build
                '''
            }
        }
        stage('E2E') {
            agent {
                docker {
                    image 'mcr.microsoft.com/playwright:v1.48.1-noble'
                    reuseNode true
                    args '-u root:root'
                }
            }
            steps {
                sh '''
                    npm install -g serve
                    serve -s build
                    npx playwright test
                '''
            }
        }
    }
    */
}
