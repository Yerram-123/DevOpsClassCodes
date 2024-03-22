pipeine { 
   agent any 
  tools { 
    jdk 'myjava -- jdk8' 
    maven 'mymaven' 
  } 
  stages { 
    stage('Clonerepo') {
      steps { 
        git 'https://github.com/Yerram-123/DevOpsClassCodes.git' 
      } 
    } 
    stage('Compile') {
      steps { 
         sh 'mvn compile' 
      } 
    }  
    stage('CodeReview') {
      steps { 
         sh 'mvn pmd:pmd'  
      } 
    }   
    stage('UnitTesting') {
      steps { 
         sh 'mvn test' 
      } 
    }   

  } 
} 
