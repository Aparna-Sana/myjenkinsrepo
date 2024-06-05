pipeline{
      agent any
      //agent { docker {image 'maven:3.6.3' }}
      //agent { docker {image 'node:20.4' }}
      stages{
            stage('Build'){
                  steps{
                        //sh 'mvn --version'
                        //sh 'node --version'
                        echo "building an application"
                        echo "$PATH"
                        echo "BUILD_NUMBER - $env.BUILD_NUMBER"
                        echo "$env.BUILD_ID"
                        echo "$env.JOB_NAME"
                        echo "$env.BUILD_TAG"
                        echo "$env.BUILD_URL"
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
      


