// Filename: Jenkinsfile
node {
  def GITREPOREMOTE = "https://github.com/dvl-samir-shinde/learning_test.git"
  def GITBRANCH     = "main"
  def DBCLIPATH     = "/home/linuxbrew/.linuxbrew/bin"
  def BUNDLETARGET  = "dev"

  stage('Checkout') {
    git branch: GITBRANCH, url: GITREPOREMOTE
  }
  
  stage('validate')
   sh"""
    ${DBCLIPATH}/databricks  bundle validate
  
   """
}
