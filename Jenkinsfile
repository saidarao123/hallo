pipeline {
    agent any
    stages {
        stage ('Clone') {
            steps {
                git branch: 'master', url: "https://github.com/viswanathkatta/mahendra.git"
            }
        }
                stage ('Exec Maven') {
            steps {
                rtMavenRun (
                    tool: maven // Tool name from Jenkins configuration
                    pom: 'pom.xml',
                    goals: 'clean install',
                    deployerId: "MAVEN_DEPLOYER",
                    resolverId: "MAVEN_RESOLVER"
                )
            }
        }

    }
}
