pipeline {
    agent any
    stages {
        stage('hello AWS') {
            steps {
                withAWS(credentials: 'aws-personal', region: 'eu-west-2') {
                    s3Upload acl: 'Private', bucket: 'formarc.net', file: 'index.html'
                                        
                    
                }
            }
        }
    }
}
