
pipeline {
    agent any

    stages {
        stage('Clone GitHub Repository') {
            steps {
                script {
                    git branch: 'main',  url: "https://github.com/ShZahid/react-Calculator/"
                }
            }
        }

        stage('Update Index.html') {
            steps {
                script {
                    sh 'rm /var/www/html/index.html'
                    sh 'cp -r * /var/www/html/'
                }
            }
        }
    }
}
