node {
  stage ('Build') {
    git url: 'https://github.com/raina564/SampleProject'
    withMaven(maven: 'M3', mavenSettingsConfig: '134446fb-7788-4708-84ab-debcb535d64a') {
      echo 'Sample Project'
      sh "mvn compile"
      sh "mvn exec:java -Dexec.mainClass=SampleClass"
    } // withMaven will discover the generated Maven artifacts, JUnit Surefire & FailSafe reports and FindBugs reports
  }
}
