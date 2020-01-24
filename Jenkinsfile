pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm config list' 
                sh 'npm config set -g always-auth false' 
                sh 'npm config set -g strict-ssl false' 
                sh 'npm config set proxy http://X185031:Sg2412%249@proxy-sgt.si.socgen:8080/' 
                sh 'npm config set registry http://registry.npmjs.org/' 
                sh 'npm intsall' 
            }
        }
    }
}
