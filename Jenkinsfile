node{
    stage('SCM Checkout'){
      git 'https://github.com/Nikitakumari13/DeployWarFile.git'
  }
  stage('compile-package'){
    // Get maven home path
    def mvnHome = tool name: 'Maven 3.8.4', type: 'maven'
    sh "${mvnHome}/bin/mvn package" 
  }
}
