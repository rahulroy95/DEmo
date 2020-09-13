pipeline {
         parameters {
  choice choices: ['DEV', 'MASTER', 'PROD'], description: 'testing', name: 'test'
}
         agent any
         stages {
                 stage('Build') {
                 steps {
                     echo 'Hi, Rahul. Starting to build the App.'
                          post {
                                              
                                               aborted {
                                                 // One or more steps need to be included within each condition's block.
                                               }
                                               success {
                                                 // One or more steps need to be included within each condition's block.
                                               }
                                               failure {
                                                 // One or more steps need to be included within each condition's block.
                                               }
                                               unsuccessful {
                                                 // One or more steps need to be included within each condition's block.
                                               }
                                               fixed {
                                                 // One or more steps need to be included within each condition's block.
                                               }
                                               changed {
                                                 // One or more steps need to be included within each condition's block.
                                               }
                             }

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
                                echo 'hello roy its done'
                     }

              }
}
}
