pipeline { 
    agent any  
    stages { 
        stage('Build') { 
            steps { 
               echo 'Build the project' 
                mvn clean install
            }
        }
    }
}
