def workspace
node
{
    stage('checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/pavansw/testpune.git']]])
        echo 'testrepo'
        workspace = pwd()
    }
    stage('Shell Script')
    {
        sh '''#!/bin/bash
hostname;date
'''
    }
    stage('Delivery')
    {
     echo 'we are building'   
    }
}
