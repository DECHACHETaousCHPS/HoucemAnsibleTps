node { 
 
 stage('clone') {
    
    git 'git@github.com:DECHACHETaousCHPS/HoucemAnsibleTps.git'

 }
 
  stage('Build') {
    
      sh 'sudo mvn clean install package'

 }
 
 stage('Deploy') {
    
     sh 'ansible-playbook -i hotess copy.yml'
 }
 
    
}
