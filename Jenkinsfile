pipeline{
    agent any
    environment{
        NEW_VERSION = '1.4.0'
        CREDELTIALS = '51ebb6df-9adb-49aa-8e45-0fd5cb881f58'
    }
    stages {
        stage ("git"){
            steps {
                git 'https://github.com/PhanBeo/ThanhDTg.git'
            }	
        } 
        stage ("build"){
            steps {
                echo 'building the app'
                echo "building version ${NEW_VERSION}"
            }	
        } 
        stage ("test"){
            steps {
                echo 'testing the app'
                echo "testing the ${CREDELTIALS}"
            }
        }
        stage ("deploy"){
            steps {
                withCredentials([
                    usernamePassword(credentialsId: '51ebb6df-9adb-49aa-8e45-0fd5cb881f58', 
                    passwordVariable: 'dau020319', 
                    usernameVariable: 'thanhdtg')])
                echo 'deploying the app'
            }
        }
    } 
}
