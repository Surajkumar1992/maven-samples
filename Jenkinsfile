pipeline{
   agent any
   
   parameters {
        string(name: 'Branch', defaultValue: 'master', description: 'Enter the feature branch to build')
   }
   
   stages{
      stage("SCM CHECKOUT"){
            steps{
               checkout([$class: 'GitSCM', branches: [[name: '*/${params.Branch']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: 'different_directory']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/Surajkumar1992/maven-samples.git']]])
                  }
               }
            }
         }
