pipeline {
    agent any
    tools { 
        maven 'MAVEN' 

    }
         stages {
         stage ('git clone') {
            steps {
                git  'https://github.com/SandhyaNanjarapalli/assignment.git' 
            }
         }
          stage ('compile') {
            steps {
                sh "mvn compile" 
            }
         }
          stage ('test') {
            steps {
                sh "mvn test" 
            }
         }
          stage ('package') {
            steps {
                sh "mvn package" 
            }
         }
          stage ('Build') {
	    steps {
                sh "mvn install" 
            }
         }
    
    }
}

