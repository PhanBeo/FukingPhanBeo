pipeline {
    agent any
    stages{
        stage("Binh Cho Dien"){
            steps{
                ([: 'OpenShiftBuilder'])(ArtifactoryGradleBuild(buildFile: 'Fcking Binh'))
        }
        stage("Binh Mad Dog"){
            sh(script: 'echo Binh Cho Dai')
            }
        }
    }
}