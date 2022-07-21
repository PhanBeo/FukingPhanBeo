pipeline{
    agent any
    environment{
        NEW_VERSION = '1.4.0'
        SERVER_CREDENTIALS = 'credentials:51ebb6df-9adb-49aa-8e45-0fd5cb881f58'
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
            }
        }
        stage ("deploy"){
            steps {
               echo "deploying with ${SERVER_CREDELTIALS}"
            }
        }
    } 
}
