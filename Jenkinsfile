pipeline {
    agent { docker { image 'maven:3.3.3' } }
    parameters {
        booleanParam(name: 'BOOLPARAM', defaultValue: true, description: 'Toggle this value')
    }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
                sh 'ls -l'
                sh 'echo Param = ${BOOLPARAM}'
            }
        }
    }
}