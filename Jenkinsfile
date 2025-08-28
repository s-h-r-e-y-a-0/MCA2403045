pipeline {
    agent any
parameters {
  string(name: 'BUILD_NUMBER_INPUT', defaultValue: '1', description: 'Enter build number for deploy step')
}
    stages {
        stage('Build') {
            when {
                branch 'development'
            }
            steps {
                echo "Running build step on development branch"
            }
        }

        stage('Test') {
            steps {
                echo "Running tests for all branches"
              
            }
        }

        stage('Deploy') {
            steps {
            echo "Deploying build number: ${params.BUILD_NUMBER_INPUT}"

            }
        }
    }
}
