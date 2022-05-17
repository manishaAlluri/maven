node{
   stage('SCM Checkout'){
   git 'https://github.com/manishaAlluri/maven/'
   }
   stage('compile-package') {
   def mvnHome = tool name: 'maven3', type: 'maven'
   sh "${mvnHome}/bin/mvn package"
   }
    stage('deploy-package') {
   sh 'cp /gitproject/target/myweb-0.0.7-SNAPSHOT.war  TOMCAT_DIRECTORY/webapps'
   }
}
