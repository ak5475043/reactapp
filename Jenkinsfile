pipeline {
    agent any
    stages {
        stage('Capture Webhook Payload') {
            steps {
                script {
                    // Capture the raw HTTP request body (payload)
                    def payloadString = env.BODY

                    // Print the payload to the Jenkins build log
                    echo "Webhook Payload:\n${payloadString}"
                }
            }
        }
    }
}


