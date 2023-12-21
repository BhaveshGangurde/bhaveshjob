pipeline {
  agent any
   stages {
         stage('Git clone') {
           steps {
               git branch: 'main', credentialsId: 'Jenkins-Github', poll: false, url: 'https://github.com/BhaveshGangurde/bhaveshjob.git'
           }
         }
        stage('Deploy') {
          steps {
            sh 'sudo cp index.html /var/www/html'
          }
        }
   }
}

     
