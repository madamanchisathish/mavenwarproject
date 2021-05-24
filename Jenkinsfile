    pipeline  {
    agent any
    stages {
    stage ('compile stage') {
    steps {
    withmaven(maven: 'MAVEN-3.8.1') {
    sh 'mvn clean compile'
    }
   }
  }
   stage ('testing stage') {
   steps {
  withmaven(maven: 'MAVEN-3.8.1') {
  }
 }
}
  stage ('deployment stage') {
  steps {
  withmaven (maven: 'MAVEN-3.8.1') {
  sh 'mvn deploy'
  }
 }
}
}
}
