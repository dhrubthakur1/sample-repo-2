pipeline {
    agent any

    stages {
        stage('Read File') {
            steps {
             /*script {
              def fileContent = readFile 'README.md'
              echo(fileContent)
              }*/
              sh "printenv"
              dir(GIT_URL.substring(url.lastIndexOf("/")+1, GIT_URL.lastIndexOf("."))){
                }
              sh "cat README.md"
            }
        }
    }
}
