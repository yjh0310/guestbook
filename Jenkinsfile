
            }
        }
        stage('Unit Test') {
            agent { label 'agent1' }
            steps {
                sh './mvnw test'
            }

            post {
                always {
                    junit '**/target/surefire-reports/TEST-*.xml'
                }
            }
        }

