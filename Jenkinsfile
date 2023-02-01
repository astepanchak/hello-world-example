node('built-in') {
    checkout scm
    stage('build') {
        withMaven(jdk: 'Default Java', maven: 'Default Maven') {
            sh 'echo JAVA_HOME=$JAVA_HOME'
            sh 'mvn clean install'
        }
    }
}