pipeline {
    agent any
    stages {
        stage('periodic Build') {
            steps {
                echo "Build image........"
                sh 'docker build -t front:test2 .'
                echo "Starting container...."
                sh 'docker run -ti -d -p 3002:3000 front:test2'
            }
        }
    }
}

