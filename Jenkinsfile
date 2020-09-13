pipeline {
         parameters {
  choice choices: ['DEV', 'MASTER', 'PROD'], description: 'testing', name: 'test'
}
         agent any
         stages {
                 stage('Build') {
                 steps {
                     echo 'Hi, Rahul. Starting to build the App.'
                 }
                 }
                 stage('Test') {
                 steps {
                    input('Do you want to proceed?')
                          checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/rahulroy95/Hello_World_Java.git']]])
                 }
                 }
                 stage('Deploy this') {
                 parallel {
                            stage('Deploy start ') {
                           steps {
                                input('Do you want to proceed?')
                                echo "Start the deploy .."
                           }
                           }
                            
                           }
                           }
                 stage('Prod') {
                     steps {
                                echo "App is Prod Ready"
                              }

              }
}
}
