node {
    stage('Git') {
        git branch: 'master', url: 'https://github.com/daticahealth/java-tomcat-maven-example.git'
    }
    stage('Maven') {
         sh 'mvn package'
    }
    stage('Archive') {
        archiveArtifacts artifacts: 'target/*.war', followSymlinks: false
    }
}

