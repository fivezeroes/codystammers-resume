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
             sh 'cp /var/jenkins_home/workspace/codystammers-resume_master/resume.pdf /home'
         }
      }
   }
}
