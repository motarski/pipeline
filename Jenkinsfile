// Script //
node {
  milestone()
  lock("Job input"){
  milestone(1)
  stage("build") {
  def hello = "Mr.Ivan"
  checkout scm
  echo "Hello ${hello}"
  echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
  input('Waiting for manual input before going to deploy stage')
  build job: 'runMe'
}
  milestone()
  stage("Deploy") {
  echo "Deploying"
  }
 }
}
