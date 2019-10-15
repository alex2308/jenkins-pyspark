node {
    stage('checkout'){
    checkout scm
    }
   stage('compile') {
         echo "compiling python project"
         sh 'pip install -r requirements.txt'
      }
   stage('test') {
      echo "Testings python project"
      sh "pytest"
   }

}