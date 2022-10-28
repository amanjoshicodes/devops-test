@Library("shared-libs") _

pipeline {
    agent any

    stages {
        
        stage('Build_Project') {
            steps {
                echo 'Building whole project here!'
                sayHello()
                saySuccess()
//                 sayFailure()
            }
            post {
                success {
                    echo 'Succeeded in Build_Project Stage.'
                }
                failure {
                    echo 'Failed in Build_Project Stage.'
                }
            }
        }
        
        stage('Parallel Stage') {
            parallel {
                stage('Test_A') {
                    steps {
                        echo 'Testing_A on project here!'
                        sayHello()
                        saySuccess()
                    }
                    post {
                        success {
                            echo 'Succeeded in Test_A Stage.'
                        }
                        failure {
                            echo 'Failed in Test_A Stage.'
                        }
                    }
                }
                
                stage('Test_B') {
                    steps {
                        echo 'Test_B on project here!'
                        sayHello()
                        saySuccess()
                    }
                    post {
                        success {
                            echo 'Succeeded in Test_B Stage.'
                        }
                        failure {
                            echo 'Failed in Test_B Stage.'
                        }
                    }
                }
                
                stage('Test_C') {
                    steps {
                        echo 'Test_C on project here!'
                        sayHello()
                        saySuccess()
                    }
                    post {
                        success {
                            echo 'Succeeded in Test_C Stage.'
                        }
                        failure {
                            echo 'Failed in Test_C Stage.'
                        }
                    }
                } 
                
            }
        }
    }
}
