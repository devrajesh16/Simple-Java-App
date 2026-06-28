pipeline {
    agent any
    tools {
        maven 'maven3.9.14'  // Use the Maven tool installed earlier
        jdk 'java17'        // Use JDK 17
    }
    stages {
        stage('Checkout') {
            steps {
                // Checkout the project from the 'project-1' branch in your GitHub repository
                git branch: 'project-1', url: 'https://github.com/devrajesh16/zomato.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Post-Build') {
            steps {
                echo "Build completed successfully."
            }
        }
    }
}
