node { 
 
 stage('clone') {
    
    git 'https://gitlab.com/khlifidev1/projet_j2e.git'

 }
 
  stage('Build') {
    
      sh 'mvn clean install package'

 }
 
 stage('Deploy') {
    
     sh 'ansible-playbook -i hosts copy.yml' 
 }
 
    
}
