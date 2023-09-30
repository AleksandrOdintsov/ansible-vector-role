pipeline {
 agent {
  label 'jenkins-agent'
 }
 stages {
     stage ('Git download') {
         steps {
            git 'https://github.com/so121183gak/ansible-vector-role.git'
      }
    }
     stage ('Execute test') {
         steps {
            sh '''#!/bin/sh
                  pwd
                  id
                  molecule test
                  exit 0''' 
      }
    }
  }
}
