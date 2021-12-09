pipeline {
    agent any

    stages {
        stage('Read File') {
            steps {
             /*script {
              def fileContent = readFile 'README.md'
              echo(fileContent)
              }*/
              print env
              sh "cat README.md"
            }
        }
    }
}
