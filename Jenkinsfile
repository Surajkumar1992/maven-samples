pipeline{
   agent any
   
   stages{
      stage("SCM CHECKOUT"){
            steps{
               def branch=params.branch;
               checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: ${branch}]], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: 'jenkins-scripts']], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '******', url: 'https://github.com/Surajkumar1992/maven-samples.git']]]
                }
          }
      }
 }
