pipeline{
    
    agent{
   
        node{
         label 'apple'
       }
}
    
      tools{
          
          maven 'mymaven'
          jdk 'myjava'
      }
             stages{
                 
                 stage('checkout'){
                     
                     steps{
                         
                         echo 'git checkout'
                         
                         git 'https://github.com/devopsstephen/sunday.git'
                         
                     }
                     
                     
                 }
                 
                 stage('package'){
                     
                     steps{
                         
                         echo 'mvn package'
                         sh 'mvn clean package'
                     }
                 }
                 
                 stage('deploy'){
                     
                     
                     steps{
                         
                         echo "deploy war to dev"
                         
                     }
                 }
                 
                 
                 
                 
                 
                 
             }
    
}
