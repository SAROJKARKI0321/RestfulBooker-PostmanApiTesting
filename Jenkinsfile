pipeline {
    agent any

    stages {
        stage('Run Postman Tests') {
            steps {
                bat '''
                    newman run pman.json ^
                    --environment envir.json ^
                    --reporters cli,junit ^
                    --reporter-junit-export results.xml
                '''
            }
        }
    }

    post {
        always {
            junit 'results.xml'
        }
    }
}
