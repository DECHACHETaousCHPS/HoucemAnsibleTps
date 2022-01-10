node { 
 
 stage('clone') {
    
    git 'https://github.com/DECHACHETaousCHPS/HoucemAnsibleTps.git'

 }
 
  stage('Build') {
    
      sh 'sudo mvn clean install package'

 }
 
 stage('Deploy') {
    
     ansiblePlaybook become: true, playbook: 'copy.yml'
 }
 
 stage('build image') {
            
                sh 'sudo docker build -t tomcat:monappli . '

  }
  stage('Run Image') {
               
                        sh 'sudo docker run -d --name tomcatctr -p 8088:8080 tomcat:monappli'
  }



