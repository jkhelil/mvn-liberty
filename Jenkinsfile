pipeline { 
  agent none 
  stages {
    stage('test maven-nodejs') {
      agent { label 'maven' }
      steps {
        git 'https://github.com/OpenLiberty/guide-rest-intro.git'
        sh 'mvn --version && cd finish && mvn liberty:create'
      }
    }
  }
}
