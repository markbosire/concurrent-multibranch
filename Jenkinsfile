pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                lock("lock1") {
                    echo 'Using lock: lock1'
                    sh 'sleep 30'
                    echo "Build completed in ${env.BRANCH_NAME}"
                }
            }
        }
    }
}
