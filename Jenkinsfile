// Script //
def extWorkspace = exwsAllocate 'diskpool1'

node {
  exws(extWorkspace) {
  def hello = "Mr.Ivan"
  checkout scm
  echo "Hello ${hello}"
  echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
    }
}
