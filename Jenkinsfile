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
	    { steps
		{
        	  sh ' echo "hello world jags" '
		//	sh '		      folder="jenkins"
//	if ! git clone "${https://github.com/jagadeesh666/}" "${folder}" 2>/dev/null && [ -d "${folder}" ] ;
// then
  //  echo "Clone failed because the folder ${folder} exists"
 //fi '
//		      sh ' git clone "https://github.com/jagadeesh666/jenkins.git "   '
 //		    sh 'ls'
	sh ' git checkout -b master origin/master' 
		     echo "inside stage checkout"
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'jags666', url: 'https://github.com/jagadeesh666/HmrcAutomationPractice.git']]])

        echo "checkout finished"
     }
    }
    stage ("second stage111")
    {
     steps{
        echo "inside stage2 checkout running shell script"

        sh label: '', script: './script.sh'
         sh label: '', script: '/Users/jagadeeshm/.jenkins/workspace/script.sh'
        echo "executed shell script successfully"
    }
}
}
}
