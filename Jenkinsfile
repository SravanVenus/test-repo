pipeline {
    agent any
    stages {
        stage('Compile Stages') {
            steps {
                withMaven{maven : 'maven_3_8_5'} {
                    bat 'mvn clean compile'
                }
            }
        }
        stage('Test Stage') {
             steps {
                withMaven{maven : 'maven_3_8_5'} {
                    bat 'mvn test'
                }
             }
        }
        stage('Deploy Stage') {
             steps {
                withMaven{maven : 'maven_3_8_5'} {
                    bat 'mvn deploy'
                }
             }
        }
    }
}
                
                
