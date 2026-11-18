pipeline {
    agent any

    stages {
        stage('Compile') {
            steps {
                echo 'Compiling...'
                bat 'javac -d . HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Running...'
                bat 'java -cp . HelloWorld'
            }
        }
    }
}
