node { 
 
 stage('clone') {
    
    git 'https://github.com/DECHACHETaousCHPS/HoucemAnsibleTps.git'

 }
 
  stage('Build') {
    
      sh 'sudo mvn clean install package'

 }
 
 stage('Deploy') {
    
     sh 'ansible-playbook -i /etc/ansible/hosts copy.yml'
 }
 
    
}
