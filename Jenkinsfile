pipeline {
  agent any
  stages {
    stage('git') {
      steps {
        git 'https://github.com/pandian3k/Maven-Demo.git' 
      }
    }
    stage('build') {
      steps {
        bat 'mvn install'
      }
    }
    stage('deploy') {
      steps {
        sh 'cp -r "C:\\\\Program Files (x86)\\\\Jenkins\\\\workspace\\\\test 1\\\\multi-module\\\\webapp\\\\target\\\\webapp.war" "C:\\\\Program Files\\\\Apache Software Foundation\\\\Tomcat 8.5_Tomcat8-devops\\\\webapps"'
      }
    }
  }
 }
