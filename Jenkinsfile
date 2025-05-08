pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                lock("lock1") {
                    echo 'Locked printer resource'
                    sh 'sleep 10'
                    echo "Build completed in ${env.BRANCH_NAME}"
                }
            }
        }
    }
}
