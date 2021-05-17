pipeline {
    agent any
    stages {

        stage('build') {

            tools {
                jdk 'JDK-14'
            }
            steps {
                sh 'mvn clean package'
            }
        }
        stage('test') {
            tools {
                jdk 'JDK-14'
            }
            steps {
                sh 'mvn test'
            }
        }

        stage('deploy') {
            tools {
                jdk 'JDK-14'
            }
//            steps {
//                //skip for now
////                sh 'mvn deploy'
//            }
        }
    }
}
