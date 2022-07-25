pipeline {
    agent any
    parameters{
        choice (name: 'VERSION', choices: ['1.0.1', '1.0.2','1.0.3'], description:'')
        booleanParam (name: 'ExecuteTests', defaultValue: true, description:'')
    }
    stages {
        stage("build"){
            steps{
                echo 'Binh Cho Dai'
            }
        }
        stage("test"){
            when {
                expression {
                    params.ExecuteTests
                }
            }
            steps{
                echo "Binh Cho Dien"
                    }
        }
        stage("deploy"){
            steps {
                echo "deploying version ${VERSION}"
            }
        }
    }
}