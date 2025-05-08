pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                lock("lock2") {
                    echo 'Using lock: lock2'
                    sh 'sleep 30'
                    echo "Build completed in ${env.BRANCH_NAME}"
                }
            }
        }
    }
}
