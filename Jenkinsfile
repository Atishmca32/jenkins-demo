pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Running Build Stage'
                echo '32 Atish Ghanekar '
                sh 'echo Build Started'
            }
        }

        stage('Generate Report') {
            steps {
                sh '''
                echo "<html><body><h1>Jenkins Build Report-32 Atish Ghanekar</h1></body></html>" > report.html
                '''
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                mkdir -p /var/www/html
                cp report.html /var/www/html/
                '''
            }
        }
    }
}
