node {
   stage('ChecOut Code') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/kattapaa/maven-project.git'
      
   }
   stage('Build') {
       echo 'Build executed'
       withMaven(jdk: 'JDK-1.8.0.151', maven: 'Maven-3.5.2') {
       sh 'mvn compile'
     }
      
   }
   stage('Test execution'){
       echo 'Test Executed..'
   }
   stage('Results') {
     echo 'Results saved..'
   }
}
