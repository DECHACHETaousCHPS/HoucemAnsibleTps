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
 
    
}
