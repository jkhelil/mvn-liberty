pipeline { 
  agent none 
  stages {
    stage('test maven-nodejs') {
      container('maven') {
        git 'https://github.com/OpenLiberty/guide-rest-intro.git'
        sh 'cd finish && mvn liberty:create'
      }
    }
  }
}