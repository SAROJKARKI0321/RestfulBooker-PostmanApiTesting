pipeline {
    agent any
    

    stages {
        stage('Check Newman Setup') {
            steps {
                bat 'newman -v'
                bat 'npm list -g newman-reporter-html || echo "newman-reporter-html not installed"'
            }
        }

        stage('Run Postman Tests') {
            steps {
                bat '''
                    newman run pman.json ^
                    --environment envir.json ^
                    --reporters cli,junit,html ^
                    --reporter-junit-export results.xml ^
                    --reporter-html-export newman-report.html
                '''
            }
        }
    }

    post {
        always {
            junit 'results.xml'
            archiveArtifacts artifacts: 'newman-report.html', allowEmptyArchive: true
        }
    }
}

