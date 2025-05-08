pipeline {
    agent any
    stages {
        stage('Sleep') {
            steps {
                sh 'sleep 10'
                echo "Completed sleep stage in ${env.BRANCH_NAME}"
            }
        }
    }
}
