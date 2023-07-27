pipeline {
    agent any
    environment {
        // Assuming the payload is a JSON object with a key named 'repository'
        PAYLOAD = "${JSON.stringify(env.BODY)}"
        // Extract the repository URL from the payload using a Groovy expression
        REPO_URL = "${PAYLOAD['repository']['url']}"
        // Extract the repository name from the URL
        REPO_NAME = "${REPO_URL.split('/')[-1].split('\\.')[0]}"
    }
    stages {
        stage('Build') {
            steps {
                // Fetch the repository
                git branch: 'main', url: "${REPO_URL}"
                // Add build steps here (e.g., compiling, testing, etc.)
            }
        }
    }
}



