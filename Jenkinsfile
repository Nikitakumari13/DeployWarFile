node{
    stage('SCM Checkout'){
   git 'https://github.com/Nikitakumari13/DeployWarFile'

  }

  stage('compile-package'){

    // Get maven home path

    def mvnHome = tool name: 'mavan 3.8.4', type: 'maven'

    sh "${mvnHome}/bin/mvn package" 

  }

  //stage('Email Notification'){}


 /* stage('Deploy to Tomcat'){


    sshagent(['tomcat-dev']) {

    sh 'scp -o StrictHostKeyChecking=no target/*.war ec2-user@172.31.6.170:/opt/apache-tomcat-9.0.74/webapps'

}

  } */

}





