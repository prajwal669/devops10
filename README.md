# devops10
trigger: - main 
pool: 
name: Default  # Matches your self-hosted agent pool 
steps: - task: Maven@3 
inputs: 
mavenPomFile: 'pom.xml' 
mavenOptions: '-Xmx3072m' 
javaHomeOption: 'Path' 
jdkDirectory: 'C:\\Program Files\\Microsoft\\jdk-17.0.14.7
hotspot'  # PATH in your system 
jdkArchitectureOption: 'x64' 
publishJUnitResults: true 
testResultsFiles: '**/surefire-reports/TEST-*.xml' 
goals: 'package'
