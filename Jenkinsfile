pipeline {
  agent any
  stages {
    stage('git') {
      steps {
        git(url: 'https://github.com/pandian3k/Maven-Demo.git', branch: 'master')
		git 
      }
    }
    stage('build') {
      steps {
        bat 'mvn install'
      }
    }
    stage('deploy') {
      steps {
        sh 'cp -r \'C:\\Program Files (x86)\\Jenkins\\workspace\\pipe2\\multi-module\\webapp\\target\\webapp.war \' \'C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps\\webapp.war\''
      }
    }
  }
 }
