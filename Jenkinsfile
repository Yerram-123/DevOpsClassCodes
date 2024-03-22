pipeine { 
   agent any 
  tools { 
    jdk 'myjava' 
    maven 'mymaven' 
  } 
  stages { 
    stage('Clonerepo') {
      steps { 
        git 'https://github.com/Yerram-123/DevOpsClassCodes.git' 
      } 
    } 
    stage('DevCompile') {
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
