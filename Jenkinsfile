node{
   stage('SCM Checkout'){
     git 'https://github.com/saikumar13/Adhoc'
   }
   stage('Compile-package'){
   steps {
   dir("time-tracker/java_project_template"){
   def mvnhome = tool name: 'MAVEN3.5', type: 'maven'
   sh "${mvnhome}/bin/mvn -f time-tracker/pom.xml clean install package"    
   }
}
