
pipeline{
  agent any 
  stages {
    stage ('Groovy Practice'){
     steps {
     script {
         def tool = "Jenkins"
         def environments = [ "Development", "QA", "Production" ]
         def version = 2.0
         def servers = [
             Development : "dev-server" ,  
             QA : "qa-server" ,
             Production : "prod-server" ]  
       servers.each { environment, server ->
    echo "$environment is $server" } 
       echo "${environments[0]}"
       echo "${environments[1]}"
       echo "${environments[2]}"
      
       for ( environment in environments ) {
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
}





         
           

    
