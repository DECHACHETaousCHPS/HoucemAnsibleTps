node { 
 
 stage('clone') {
    
    git 'https://gitlab.com/khlifidev1/projet_j2e.git'

 }
 
  stage('Build') {
    
      sh 'sudo mvn clean install package'

 }
 
 stage('Deploy') {
    
     sh 'ansible-playbook -i hotess copy.yml'
 }
 
    
}
