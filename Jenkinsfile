node {
  def mavenHome = tool name: 'maven3.8.5', type: 'maven'
  stage("git checkout") {
     git  'branch: main', url: 'https://github.com/maheshpothuganti/zamzamrepo.git'
  }
  stage("maven build"){
  sh '${mavenHome}/bin/mvn clean package'
  }
}
