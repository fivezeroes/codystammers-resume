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
             sh 'cp /var/jenkins_home/codystammers-resume/resume.pdf /home'
         }
      }
   }
}
