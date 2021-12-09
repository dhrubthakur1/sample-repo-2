pipeline {
    agent any

    stages {
        stage('Read File') {
            steps {
             /*script {
              def fileContent = readFile 'README.md'
              echo(fileContent)
              }*/
              cat README.md
            }
        }
    }
}
