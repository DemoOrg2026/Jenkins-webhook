def workspace
node
{
    stage('checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/DemoOrg2026/Jenkins-webhook.git']]])
        workspace = pwd()
    }
    stage('static code analysis')
    {
        echo 'Code analysis stage'
    }
    stage('Build')
    {
        echo 'Building stage'
    }
    stage('Unit testing')
    {
        echo 'Unit testing'
    }
    stage('Delivery')
    {
        echo 'Delivery stage'
    }
}
