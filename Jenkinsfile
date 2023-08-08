pipeline {
  agent any
  triggers {
    githubPush()
  }
     stages {
        stage("Build") {
            steps {
                sh "chmod +x -R ${env.WORKSPACE}"
                sh '/var/lib/jenkins/workspace/cicd10/deploy.sh'
            }
        }
    }
}
