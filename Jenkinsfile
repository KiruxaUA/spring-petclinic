pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'make'
            }
        }
    }
    triggers {
        // Build whenever changes are pushed to any branch
        branch('*') {
            build(true)
        }
    }
}
