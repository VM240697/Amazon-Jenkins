pipeline {
    agent any
       
    stages {

        stage('pull scm') {
            steps {
                git branch: 'dev', url: 'https://github.com/VM240697/Amazon-Jenkins'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
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
