pipeline {
    agent any

    environment {
        PROJECT_DIR = '/Users/koonqi/Library/CloudStorage/OneDrive-UniversitiTunkuAbdulRahman/UTAR/Semester 8/Software Construction And Configuration/Assignment/Assignment 1/SCC-1'
    }

    tools {
        gradle "gradle"
    }

    stages {
        stage('Build') {
            steps {
                dir(PROJECT_DIR) {
                    sh './gradlew clean build'
                }
            }
        }
        stage('Test') {
            steps {
                dir(PROJECT_DIR) {
                    sh './gradlew test'
                }
            }
        }

    }
}
