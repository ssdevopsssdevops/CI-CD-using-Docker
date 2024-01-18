pipeline {
    agent any
	
	  tools
    {
       maven "Maven"
    }
 stages {
      stage('checkout') {
           steps {
             
                sh 'ls'
             
          }
        }
	 stage('Execute Maven') {
           steps {
             
                sh 'mvn package'             
          }
        }
        

stage('build to develop') {
              when {
                  branch 'master'             
              }
              steps {
                 echo "Working on master branch"
              }
         }
     
 
     
 

    }
	}
    
