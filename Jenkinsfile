pipeline{
     agent any
     stages{
          stage("Checkout"){
               git branch: "main", url: "https://github.com/khaleel009/Maven-Pipeline-Project.git"
          }
          stage("Build"){
               sh 'mvn clean package'
               sh 'java -cp target/awesome-stylish-maven-project-1.0-SNAPSHOT.jar com.example.app.Main'
          }
     }
}