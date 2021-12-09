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
                echo "${GIT_URL}"
                echo GIT_URL.substring(GIT_URL.lastIndexOf('/')+1, GIT_URL.lastIndexOf('.'))
             // dir("${GIT_URL}".substring("${GIT_URL}".lastIndexOf("/")+1, "${GIT_URL}".lastIndexOf("."))){
                dir('Test') {
                }
              sh "cat README.md"
            }
        }
    }
}
