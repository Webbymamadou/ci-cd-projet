pipeline {
    agent any

    stages {
        stage ('test'){
            echo 'Installation des dependences'
            sh 'pip install -r requirements.txt'

            echo 'Lancement des test'
            sh 'pytest'
        }

    }
}