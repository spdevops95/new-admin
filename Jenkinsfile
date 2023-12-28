pipeline {
    agent {
        kubernetes {
            label 'test1-${BUILD_ID}'
            defaultcontainer "test1"
            yamlFile 'deployment.yml'
        }   
    }
    
    environment {
        //PATH = "/usr/local/bin:$PATH"
    }

    stages {
        stage('Build') {
            steps {
                echo 'Executing the build command...'
                
                // Replace 'your_build_command' with the actual build command
            }
        }

        stage('Test') {
            steps {
                echo 'Executing the test command...'
            
                // Replace 'your_test_command' with the actual test command
            }
        }

        stage('Deploy') {
            steps {
                echo 'Executing the deployment command...'
                
                // Replace 'your_deploy_command' with the actual deployment command
            }
        }
    }

    post {
        success {
            echo 'Pipeline succeeded! Ready for the next steps.'
            // Add success post-build actions here
        }
        failure {
            echo 'Pipeline failed. Please check the logs.'
            // Add failure handling or notifications here
        }
    }
}
