pipeline {
    agent any

    stages {

        stage('Fetch Files') {
            steps {
                git branch: 'main', 
                    url: 'https://github.com/Yash-Singh0408/jeck_git.git'
            }
        }

        stage('Building') {
            steps {
                echo 'Building Project'
                bat 'javac test1.java'
            }
        }

        stage('Executing') {
            steps {
                echo 'Executing Project'
                bat 'java test1'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying Project'
            }
        }

    }
}
