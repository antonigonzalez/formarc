pipeline {
    agent any
    stages {
        stage('hello AWS') {
            steps {
                withAWS(credentials: 'aws-personal', region: 'eu-west-2') {
                    s3Upload(bucket:"formarc.net", workingDir:'', includePathPattern:'**/*');
                                        
                    
                }
            }
        }
    }
}
