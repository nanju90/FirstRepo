node {
    def rtMaven = Artifactory.newMavenBuild()
    def buildInfo

    stage ('Clone') {
        git url: 'https://github.com/nanju90/FirstRepo.git'
    }

    stage ('Artifactory configuration') {
        rtMaven.tool = maven_3_5_2 // Tool name from Jenkins configuration
        buildInfo = Artifactory.newBuildInfo()
    }

    stage ('Exec Maven') {

        rtMaven.run pom: 'FirstRepo/pom.xml', goals: 'clean install', buildInfo: buildInfo
    }

 }
