pipeline{
   agent any
   
   stages{
      stage("SCM CHECKOUT"){
            steps{
               def Branch=${params.Branch};
                  checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: '${Branch}']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: 'jenkins-scripts']], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'SurajKumar1992', url: 'https://github.com/Surajkumar1992/maven-samples.git']]]
                  }
               }
            }
         }
