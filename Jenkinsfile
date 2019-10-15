node {
    stage('checkout'){
    checkout scm
    }
   stage('build image') {
         echo "building docker image"
         sh 'pip3 install -r requirements.txt'
      }
   stage('test') {
      echo "running test through docker"
      sh "pytest"
   }

}
