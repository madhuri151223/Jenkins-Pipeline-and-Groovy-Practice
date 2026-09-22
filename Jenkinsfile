
pipeline{
  agent any 
  stages {
    stage ('Groovy Practice'){
     steps {
     script {
         def tool = "Jenkins"
         def environment = "QA"
         def version = 2.0
         if (environment == "Development") {
           echo("Deploying to Development")
         }
         else if (environment == "QA") {
           echo("Deploying to QA")
         }
          else if (environment == "Production") {
            echo("Production requires manual approval")   
          }
       }
     }
  }
}
}






         
           

    
