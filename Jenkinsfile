pipeline {
  agent any
  stages {
    stage('git checkout') {
      steps {
        git(url: 'https://github.com/jnmullen/hello-world-spring-boot', branch: 'master')
      }
    }
    stage('maven') {
      steps {
        sh 'mvn -B -DskipTests clean package'
      }
    }
  }
}