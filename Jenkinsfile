pipeline { 
  agent none 
  stages {
    container('maven') {
        git 'https://github.com/OpenLiberty/guide-rest-intro.git'
        sh 'cd finish && mvn liberty:create'
    }
  }
}