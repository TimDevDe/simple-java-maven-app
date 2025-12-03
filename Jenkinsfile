pipeline {
    // This directive tells Jenkins to run the entire pipeline on the agent labeled 'maven'
    agent {
        label 'maven'
    }
    stages {
        stage('Build') {
            steps {
                // This command will now run inside the correct container that has Maven installed
                sh 'mvn -B -DskipTests clean package'
            }
        }
        // ... rest of your stages
    }
}
