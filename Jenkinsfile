    pipeline  {
    agent any
    stages {
    stage ('compile stage') {
    steps {
    withmaven(maven: 'MAVEN-3.5.0') {
    sh 'mvn clean compile'
    }
   }
  }
   stage ('testing stage') {
   steps {
  withmaven(maven: 'MAVEN-3.5.0') {
  }
 }
}
  stage ('deployment stage') {
  steps {
  withmaven (maven: 'MAVEN-3.5.0') {
  sh 'mvn deploy'
  }
 }
}
}
}
