pipeline {
    agent any
           stages {

        stage('pull scm') {
            steps {
                git branch: 'vijay', url: 'https://github.com/VM240697/Amazon-Jenkins'
            }
        }
        stage('Install') {
            steps {
                sh 'mvn install'
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
