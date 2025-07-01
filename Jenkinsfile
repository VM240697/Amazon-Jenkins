pipeline {
    agent any
       }
    stages {

        stage('pull scm') {
            steps {
                git branch: 'main', url: 'https://github.com/VM240697/Amazon-Jenkins'
            }
        }
        stage('Clean') {
            steps {
                sh 'mvn clean'
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
