node {
  stage ('hello') {
    dir ('foo') {
      checkout([$class: 'GitSCM', branches: [[name: 'features/this-bug']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'LocalBranch', localBranch: 'features/this-bug']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/MRamonLeon/fndjen-1842.git']]])
      echo 'Hello first commit'
    }
  }
}