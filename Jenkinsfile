
pipeline{
  agent any 
  stages {
    stage ('Groovy Practice'){
     steps {
     script {
         def tool = "Jenkins"
         def environments = [ "Development", "QA", "Production" ]
         def version = 2.0
       echo "${environments[0]}"
       echo "${environments[1]}"
       echo "${environments[2]}"
         if (environments == "Development") {
           echo("Deploying to Development")
         }
         else if (environments == "QA") {
           echo("Deploying to QA")
         }
          else if (environments == "Production") {
            echo("Production requires manual approval")   
          }
       }
     }
  }
}
}






         
           

    
