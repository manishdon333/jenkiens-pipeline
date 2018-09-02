pipeline {
        agent any
        stages {
            stage('Compile stage') {
                steps {
                    maven(maven : 'maven_3_5_4'){
                        bat "mvn clean compile"
                }
            }
        }

             stage('testing stage') {
                 steps {
                    maven(maven : 'maven_3_5_4'){
                        bat "mvn test"
                }
            }
        }

              stage('deployment stage') {
                  steps {
                    maven(maven : 'maven_3_5_4'){
                        bat "mvn deploy"
                }
            }
        }

      }

    }
I