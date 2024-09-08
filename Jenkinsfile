pipeline {
            agent { label 'Jenkins nodes' }
            tools {
                      maven 'mvn3.9'
            }
        stages {
              stage('source') { 
                  steps { 
                      git url:"https://github.com/Nisarga23nisu/simple-java-maven-app.git"
                        branch 'master'
                  }
              }
        stage ('package'){
               steps{
                        sh 'mvn package' 
            }
        }
        stage ('archiveArtifact'){
               steps{
                        archiveArtifacts artifacts: "target/my-app-1.0-SNAPSHOT.jar"
            }
        }
     }   
}

