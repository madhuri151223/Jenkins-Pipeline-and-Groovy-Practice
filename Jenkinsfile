
pipeline{
  agent any 
  stages {
    stage ('Groovy Practice'){
     steps {
     script {
         def tool = "Jenkins"
         def services = [ "payment-service",
                          "order-service",
                          "user-service"
                        ]
         def DeployEnvironments = [ "Development",
                                    "QA",
                                    "Production", 
                                    "DR"
                                  ]
       def deployApp(service, DeployEnvironment) {
         echo "deploying ${service} to ${DeployEnvironment}"
       }
       
       for ( service in services ) {
         for ( DeployEnvironment in DeployEnvironments ) {
    deployApp(service, DeployEnvironment)
           
       }
           
         
       }

// YOUR CODE
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





         
           

    
