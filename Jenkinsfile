pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                checkout scmGit(branches: [[name: '**']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/coach4u/testproject.git']])
                
            }
    }
        stage('Ruuning code') {
            steps {
               sh '''chmod +x script.sh
                bash script.sh'''
           }
       }
   }
}
