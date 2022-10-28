@Library("shared-libs") _

pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                sayHello()
                saySuccess()
//                 sayFailure()
            }
            post {
                success {
                    echo 'Succeeded in Hello Stage.'
                }
                failure {
                    echo 'Failed in Hello Stage.'
                }
            }
        }
    }
}
