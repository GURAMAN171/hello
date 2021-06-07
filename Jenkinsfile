pipeline {
   agent any
   stages {
    stage('Checkout') {
      steps {
        script {
           // The below will clone your repo and will be checked out to master branch by default.
           
           git credentialsId: 'c36caad4-5712-4efb-a233-d83865d44f8f', url: 'https://github.com/GURAMAN171/hello.git'
           // Do a ls -lart to view all the files are cloned. It will be clonned. This is just for you to be sure about it.
           
           sh "pwd"
           sh "ls -lart ./*" 
           // List all branches in your repo. 
           sh "git branch -a"
           // Checkout to a specific branch in your repo.
           sh "git checkout branchname"
          }
       }
    }
  }
}
