pipeline
{
agent any
  
  tools
  {
     nodejs 'node'
  }
  stages
  {
  stage('Build')
    {
    steps
      {
      script
        {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/arunyogi11/react-web-app.git']]])
        }
      }
    }
  }
}
