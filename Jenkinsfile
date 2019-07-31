pipeline {
   agent none
   stages {
      stage('Build') {
         agent {
            docker {
               image 'blang/latex:ubuntu'
            }
         }
         steps {
             sh 'xelatex resume.tex'
         }
      }
   }
}