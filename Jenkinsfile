pipeline {
            agent { label 'Jenkins-demo' }
            tools {
                      maven 'mvn3.9'
            }
        stages {
              stage('source') { 
                  steps { 
                      git url:"https://github.com/Nisarga23nisu/simple-java-maven-app.git"
                        branch: 'master'
        stages ('package'){
               steps{
                        sh 'mvn package' 
            }
        }
     }   
  }
}
}
