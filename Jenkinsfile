pipeline {
 agent {
  label 'ansible'
 }
 stages {
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
