node {
    stage('checkout'){
    checkout scm
    }
   stage('build image') {
         echo "building python dependencies"
         sh 'pip install -r requirements.txt'
      }
   stage('test') {
      echo "running test through docker"
      sh "pytest"
   }

}
