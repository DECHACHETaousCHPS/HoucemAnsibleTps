node { 
 
 stage('clone') {
    
    git 'https://github.com/DECHACHETaousCHPS/HoucemAnsibleTps.git'

 }
 
  stage('Build') {
    
      sh 'sudo mvn clean install package'

 }
 
 stage('Deploy') {
    
     sh 'sudo ansible-playbook -b copy.yml'
 }
 
    
}
