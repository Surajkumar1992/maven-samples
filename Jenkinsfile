pipeline{
   agent any
   
   parameters {
        string(name: 'Branch', defaultValue: 'master', description: 'Enter the feature branch to build')
   }
   
   stages{
      stage("SCM CHECKOUT"){
            steps{
                  checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: ${params.Branch}]], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: 'jenkins-scripts']], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'SurajKumar1992', url: 'https://github.com/Surajkumar1992/maven-samples.git']]]
                  }
               }
            }
         }
