node {
    stage('checkout') {
      checkout scm
    }
    stage('build packer') {
      sh """
        wget https://releases.hashicorp.com/packer/1.2.3/packer_1.2.3_linux_amd64.zip
        tar xvf packer_1.2.3_linux_amd64.zip
        cd packer_1.2.3_linux_amd64
        packer build
      """
    }
    stage('done') {
      echo "Done packer is built"
    }
}
