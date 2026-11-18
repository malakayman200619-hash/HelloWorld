pipeline {
    agent any

    stages {
        stage('Compile') {
            steps {
                echo 'Compiling...'
                bat 'dir'
                bat 'type HelloWorld.java'
                bat 'javac -verbose -d . HelloWorld.java'
                bat 'dir /s /b *.class'
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
