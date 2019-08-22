pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {
               
                bat "mvn  clean"
            }
        }
        stage('Compile') {
            steps {
                
                bat "mvn  install"
            }
        }
        stage('Test') {
            steps {
                
                 echo 'Test Completed!' 
            }
        }
        stage('Deploy') {
            steps {
                
                bat "copy enterprise_errorlogger_service\\target\\enterprise_errorlogger-1.0.0-SNAPSHOT-mule-application.jar F:\\mule_server\\mule-enterprise-standalone-4.2.1\\apps"
            }
        }
    }
<<<<<<< HEAD
}
=======
}
>>>>>>> cc7420b72082e3df3df3e4b76d86934aed99437a
