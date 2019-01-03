# simple-python-pyinstaller-app

Fue modificado y lo que hace es ejecutar python y mostrar su version
ejecuta un container con python 
como lo hizo , ni idea? , por ahora

ejemplo del archivo Jenkinsfile:

pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('build') {
            steps {
               sh  'python --version'
            }
        }
    }
}
