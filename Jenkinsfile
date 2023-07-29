pipeline {
    agent {
		label 'master'
	}

    stages {
        stage('checkout') {
            steps {
                git credentialsId: 'GIT_LOGIN', url: 'https://github.com/khaleelmo/webapp'
                //bat 'dotnet build -c Release'
             
				//input 'okay to Proceed?'
            }
        }
        
         stage('build') {
		 when{
			branch 'master'
		 }
		 
            steps {
                
                echo 'in builld'
                
            }
        }
        
        stage('Test') {
            steps {
                
                echo 'in Test'
                
            }
        }
    }
}
