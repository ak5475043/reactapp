pipeline {
    agent any
    environment {
        // Access the webhook payload using the environment variable PAYLOAD
        PAYLOAD = "${JSON.stringify(env.BODY)}"
        // Extract the repository name from the payload using a Groovy expression
        REPO_NAME = "${PAYLOAD.split('/')[5].split('.')[0]}"
    }
    stages {
        stage('Build') {
            steps {
                // Fetch the repository
                git branch: 'main', url: "https://github.com/your-username/${REPO_NAME}.git"
                // Add build steps here
            }
        }
    }
}


