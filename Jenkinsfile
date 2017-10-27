node {
	stage ('Clone') {
        git url: 'https://github.com/nanju90/FirstRepo.git'
    }
	stage ('Exec Maven') {
		rtMaven.tool = MAVEN_TOOL // Tool name from Jenkins configuration
        rtMaven.run pom: 'maven-example/pom.xml', goals: 'clean install', buildInfo: buildInfo
    }
}
