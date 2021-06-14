node {
  stage ('Build') {
    git url: 'https://github.com/raina564/SampleProject'
    withMaven {
      sh "mvn clean"
    } // withMaven will discover the generated Maven artifacts, JUnit Surefire & FailSafe reports and FindBugs reports
  }
}
