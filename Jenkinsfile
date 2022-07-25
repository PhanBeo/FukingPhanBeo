pipeline {
    agent any
    stages {
        stage("run frontend"){
            steps{
                echo "executing yarn"
                nodejs('NodeJs') {
                    sh 'install yarn'
                }
            }
        }
        stage("run backend"){
            steps{
                echo "executing gradle"
                withGradle(){
                    sh './gradlew -v'
                }
            }
        }
    }
}