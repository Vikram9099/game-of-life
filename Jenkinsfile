node {
    stage('SCM'){
        // git clone 
            git 'https://github.com/asquarezone/game-of-life.git'
    }
    stage ('build the package') {
        // mvn package
            sh 'mvn package'
    }
    stage ('Results'){
        archive 'gameoflife-web/target/gameoflife.war'
        junit 'gameoflife-web/target/surefire-reports/*.xml'
    }
}
