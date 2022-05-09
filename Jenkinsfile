node{
   agent('SCM Checkout'){
   git 'https://github.com/manishaAlluri/maven/'
   }
   agent('compile-package') {
   def mvnHome = tool name: 'maven3', type: 'maven'
   sh "${mvnHome}/bin/mvn package"
   }
}
