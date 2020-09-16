 node {
   stage ('Checkout the code')
		  {
     checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/muntasirg/Renewables.git']]])
          }
          
   }