pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Git clone') {
            steps {
                git branch: 'master', url: 'https://github.com/makgab/GitTest.git'
            }
        }
    }
}
