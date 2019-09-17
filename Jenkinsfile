node {
properties([parameters([choice(choices: ['DEV', 'MASTER'], description: '', name: 'DEV')])])
    stage 'Checkout from GitLab'
        echo 'Checking out files'
       checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '5f160068-5444-48ee-b238-a6e808a748b7', url: 'https://github.com/rahulroy95/DEmo.git']]])
        }

