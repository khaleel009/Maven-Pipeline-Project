pipeline{
     agent { label 'slavenode' }
     tools { maven 'maven-3.9.9' }
     stages{
          stage("Checkout"){
               steps{
               git branch: "main", url: "https://github.com/khaleel009/Maven-Pipeline-Project.git"
          }
          }
          stage("Build"){
               steps{
               sh 'mvn clean package'
               sh 'java -cp target/awesome-stylish-maven-project-1.0-SNAPSHOT-shaded.jar com.example.app.Main'
          }
          }
     }
}