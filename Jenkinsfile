pipeline{
      agent any
      // agent { docker {image 'maven:3.6.3' }}
      // agent { docker {image 'node:20.4' }}

      environment {
                  dockerHome = tool 'myDocker'
                  mavenHome = tool 'myMaven'
                  PATH = '$dockerHome/bin:$mavenHome/bin:$PATH'
            }

      stages{
            
            stage('Build'){
                  steps{
                        //sh 'mvn --version'
                        //sh 'node --version'
                        echo "building an application"
                        echo "$PATH"
                        echo "BUILD_NUMBER - $env.BUILD_NUMBER"
                        echo "BUILD_ID - $env.BUILD_ID"
                        echo "JOB_NAME - $env.JOB_NAME"
                        echo "BUILD_TAG - $env.BUILD_TAG"
                        echo "BUILD_URL - $env.BUILD_URL"
                        
                  }
            }
            stage('Test'){
                  steps{
                        echo "Testing an application"
                  }
            }
            stage('Deploy'){
                  steps{
                        echo "Deploying an application"
                  }
            }
            

      }

}
      


