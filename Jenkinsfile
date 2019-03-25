// Script //
node {
  stage("build") {
  def hello = "Mr.Ivan"
  checkout scm
  echo "Hello ${hello}"
  echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
  input('Waiting for manual input before going to deploy stage')
}
  stage("Deploy") {
  echo "Deploying"
  }
}
