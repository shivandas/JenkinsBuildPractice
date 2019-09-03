node('UBUNTU') {

    stage('GIT') {
        git 'https://github.com/GitPracticeRepo/JenkinsBuildPractice.git'
    }
    stage('package') {
        sh 'mvn package'
    }
    stage('archiveartifacts') {
        archive 'gameoflife-web/target/*.war'
    }
}