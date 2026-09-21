pipeline {
  agent any
  stages {
      stage('Groovy practice'){
       steps {
         script {
           def tool = "Jenkins"
          
           def environment = "Development"
           if (environment == "production") {
            echo("hello world")
            }
           def version = 1.0
        echo("I am learning $tool practicing in $environment with $version" )
         
             }
  }
  }
}
}
