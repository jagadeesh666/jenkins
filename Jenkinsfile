//script
//node {
//    echo "hello world"
 //   stage ("Checkout")
  //  {
   //     echo "inside stage checkout"
//        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'jags666', url: 'https://github.com/jagadeesh666/HmrcAutomationPractice.git']]])
//        echo "checkout finished"
 //   }
 //   stage("second stage")
//    {
//        echo "inside stage2 checkout running shell script"
//       
//        sh label: '', script: './script.sh'
//         sh label: '', script: '/Users/jagadeeshm/.jenkins/workspace/script.sh'
//        echo "executed shell script successfully"
//    }
//}

//Declarative way
pipeline {
agent any
//    echo "hello world"
    stages 
	{stage ("Checkout111")
    {
        echo "inside stage checkout"
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'jags666', url: 'https://github.com/jagadeesh666/HmrcAutomationPractice.git']]])

        echo "checkout finished"
    }
    stage ("second stage111")
    {
        echo "inside stage2 checkout running shell script"

        sh label: '', script: './script.sh'
         sh label: '', script: '/Users/jagadeeshm/.jenkins/workspace/script.sh'
        echo "executed shell script successfully"
    }
}
}
