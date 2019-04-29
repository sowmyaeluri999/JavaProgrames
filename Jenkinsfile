def workspace;
node {
   stage('checkout'){
       
       checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'sshidkey', url: 'https://github.com/sowmyaeluri999/JavaProgrames.git']]])
   workspace=pwd()
   }
   stage('Static Code Analysis'){
       echo"Static Code Analysis"
   }
   stage('Build'){
       echo"Build the code"
   }
   stage('Unit Testing'){
       echo"Unit Test"
   }
   stage('Delivery')
   {
       echo"Delivery the code"
   }
   
}
