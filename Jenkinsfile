pipeline {
    agent {
        label 'app-builder'
    }

    stages {
        stage('Build') {
            steps {
                sh 'java -version'
                sh 'mvn -version'
                sh 'echo "Maven build started at: $(date)"'
                sh 'mvn -B clean package'
                sh 'echo "Maven build completed at: $(date)"'
            }
        }
    }
}
