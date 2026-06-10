pipeline {
    agent {
        label 'app-builder'
    }

    stages {
        stage('Build') {
            steps {
                echo "Java version:"
                sh 'java -version'
                echo "Maven version:"
                sh 'mvn -version'
                echo "Maven build started at: $(date)"
                sh 'mvn -B clean package'
                echo "Maven build completed at: $(date)"
            }
        }
    }
}
