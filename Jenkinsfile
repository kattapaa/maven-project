node {
   stage('ChecOut Code') { 
      // Get some code from a GitHub repository
      git 'https://github.com/kattapaa/maven-project.git'
      
   }
   stage('Build') {
       echo 'Build executed'
       withMaven(jdk: 'OpenJDK1.8', maven: 'maven3.5.2') {
       sh 'mvn compile'
     }
      
   }
   stage('Test execution'){
       echo 'Test Executed..'
       sh 'mvn test'
   }
   stage('Results') {
     echo 'Results saved..'
   }
}
