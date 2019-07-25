node {
 
   stage('code checkout') { 
       
       git credentialsId: 'githubID', url: 'https://github.com/creativetech123/maven_apps.git'
       
   }
   
   stage('Build') {
       withMaven(jdk: 'JDK', maven: 'maven') {
    sh 'mvn clean compile'
}
     
      
   }
   
   stage('unit test') {
       withMaven(jdk: 'JDK', maven: 'maven') {
    sh 'mvn test' 
}
      
   }
   
   stage('package') {
       withMaven(jdk: 'JDK', maven: 'maven') {
    sh 'mvn package'
}
      
   }
   
   stage('deploy to dev') {
      
   }
   
   stage('deploy to test') {
      
   }
   
   stage('deploy to prod') {
      
   }
}
