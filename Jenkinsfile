pipeline {
     agent { label 'master' }
     stages {
          stage('Source') {
               steps {
                    git branch: 'main',
                        url: 'https://github.com/ladyusa/greetserver'
               }
          }
          stage('Build') {
               steps {
                    sh 'npm install'
               }
          }
          stage('Test') {
               steps {
                    echo 'testing...'
               }
          }
          stage('Performance Test') {
               steps {
                    echo 'performance testing...'
               }
          }
          stage('Deploy') {
               steps {
                    sh 'npm start'
               }
          }
     }
}
