pipeline {
  agent any
  stages {
    stage('checkout') {
      agent any
      steps {
        git(url: 'https://github.com/rajekb/sampledotnetcore.git', branch: 'main')
      }
    }

    stage('Build') {
      steps {
        bat 'dotnet build SampleConsole.csproj'
      }
    }

  }
}