node {
  stage ('hello') {
    dir ('foo') {
      checkout([$class: 'GitSCM', branches: [[name: 'features/this-bug']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'LocalBranch', localBranch: 'features/this-bug']], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'YourCreds', url: 'YourGitURL']]])
      echo 'Hello first commit'
    }
  }
}