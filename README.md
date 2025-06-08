# devops10
trigger:
  - main

pool:
  name: Default  # Matches your self-hosted agent pool

steps:
  - task: Maven@3
    inputs:
      mavenPomFile: 'pom.xml'
      mavenOptions: '-Xmx3072m'
      javaHomeOption: 'Path'
      jdkDirectory: 'C:\\Program F
