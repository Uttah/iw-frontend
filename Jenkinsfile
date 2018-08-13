pipeline {
    agent any
    stages {
        stage('nigtly Build') {
            steps {
                echo "Building image........"
                sh 'docker build -t icoworld:front-master .'
                echo "Starting container......"
                sh 'docker run -ti -d -p 3000:3000 icoworld:front-master'
            }
        }
    }
}

