pipeline {
    agent any
    stages {
        stage('hello AWS') {
            steps {
                withAWS(credentials: 'aws-personal', region: 'eu-west-2') {
                    sh 'aws s3 cp public s3://formarc.net --recursive'
                                        
                    
                }
            }
        }
    }
}
