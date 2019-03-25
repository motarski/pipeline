// Script //
node {
  lock("Job input"){
  stage("build") {
  def hello = "Mr.Ivan"
  checkout scm
  echo "Hello ${hello}"
  echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
  input('Waiting for manual input before going to deploy stage')
  build job: 'runMe'
}
  stage("Deploy") {
  echo "Deploying"
  }
 }
}
