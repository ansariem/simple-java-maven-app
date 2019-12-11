
pipeline {
    agent any
    stages {
        stage('Clean up workspace') {
            steps {
            deleteDir() /* clean up our workspace */  
            }
            }
 
        stage('Git Initialization and Check-Out') {
            steps {
            checkout scm
            }
            }
 
        stage('test Build') {
            steps {      
            sh '''
       sudo npm install -g @angular/cli
        sudo yum install -y perl
        npm get
        npm config ls -l
        npm install --verbose                 
              '''
            }
            }
