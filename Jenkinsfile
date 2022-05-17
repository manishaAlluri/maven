node{
   stage('SCM Checkout'){
   git 'https://github.com/manishaAlluri/maven/'
   }
   stage('compile-package') {
   def mvnHome = tool name: 'maven3', type: 'maven'
   sh "${mvnHome}/bin/mvn package"
   }
    stage('deploy-package') {
   sh 'cp /Users/ar7833/.jenkins/workspace/gitproject/target/myweb-0.0.7-SNAPSHOT.war  /usr/local/Cellar/tomcat@9/9.0.62/libexec/webapps/'
   }
}
