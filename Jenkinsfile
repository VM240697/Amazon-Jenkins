pipeline {
    agent any
       
    stages {

        stage('pull scm') {
            steps {
                git branch: 'Master', url: 'https://github.com/VM240697/Amazon-Jenkins'
            }
        }
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }

    }

  post{

  success{
     echo 'Build success'
  }
    
  failure{
       echo 'Failure in the build'
   }

  }


}
