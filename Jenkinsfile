
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
       curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
       sudo apt install nodejs
       sudo apt update
       sudo npm install -g @angular/cli
       sudo apt-get install perl
        npm get
        npm config ls -l
        npm install --verbose                 
              '''
            }
            }
    }
}
