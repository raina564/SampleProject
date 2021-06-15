node {
  stage ('Build') {
    git url: 'https://github.com/raina564/SampleProject'
    withMaven {
      echo 'Sample Project'
      sh "mvn compile"
      sh "mvn exec:java -Dexec.mainClass=SampleClass"
    } // withMaven will discover the generated Maven artifacts, JUnit Surefire & FailSafe reports and FindBugs reports
  }
}
