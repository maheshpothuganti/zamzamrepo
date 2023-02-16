node {
  def mavenHome = tool name: 'maven3.6.3:', type: 'maven'
  stage("git checkout") {
     git  branch: 'main', url: 'https://github.com/maheshpothuganti/zamzamrepo.git'
  }
  stage("maven build"){
     sh '${mavenHome}/bin/mvn clean test package'
  }
}
