pipeline{
   agent any
    
   tools{
      jdk "java-1.8.0-openjdk.x86_64"
   }
   
   stages{
      stage("SCM CHECKOUt){
            steps{
               def branch;
               branch=params.branch;
               checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: $(branch}]], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: 'jenkins-scripts']], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '******', url: 'https://github.com/Surajkumar1992/maven-samples.git']]]
                 }
      }
   }
 }
