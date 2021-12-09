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
              dir("${GIT_URL}".substring("${GIT_URL}".lastIndexOf("/")+1, "${GIT_URL}".lastIndexOf("."))){
                }
              sh "cat README.md"
            }
        }
    }
}
