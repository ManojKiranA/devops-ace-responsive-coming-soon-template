pipeline{
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Checkout Git Code') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/main']],
                userRemoteConfigs: [[url: 'https://github.com/ManojKiranA/devops-ace-responsive-coming-soon-template.git']]])
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
        stage('Post Deploy') {
            steps {
                echo 'Post Deploying....'
            }
        }
    }
}