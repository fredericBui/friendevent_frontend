pipeline {
    agent {
        node {
            label 'agent_nodejs'
        }
    }

    stages {
        stage('CI') {
            steps {
                git branch: 'main', url: 'https://github.com/fredericBui/friendevent_frontend.git'
            }
        }
    }
}
