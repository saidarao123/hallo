def getProjectName() {
    return 'JenkinsPipeline'
}

def getJDKVersion() {
    return ' 1.8.0_191'
}

def getMavenConfig() {
    return 'maven-config'
}

def getMavenLocation() {
    return 'M2_HOME'
}

pipeline {
    agent any 
    stages {
        stage('clone') {
            steps {
            git branch: 'master', url: "https://github.com/viswanathkatta/mahendra.git"
                }
    }
  }
}

