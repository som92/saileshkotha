node {
    stage('checkout') {
      checkout scm
    }
    stage('build packer') {
      sh """
         packer build
      """
    }
    stage('done') {
      echo "Done packer is built"
    }
}
