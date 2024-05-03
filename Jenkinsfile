pipeline { 
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/shrutisawant23/prac.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building...." // Include any build steps here
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying....'
                bat "xcopy /Y /I /E /F /C *.html C:\\xampp\\htdocs\\"
            }
        }
    }
}
