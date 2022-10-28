@Library("shared-libs") _

pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                sayHello()
                saySuccess()
                sayFailure()
            }
        }
    }
}
