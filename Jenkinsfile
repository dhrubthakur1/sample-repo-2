pipeline {
    agent any

    stages {
        stage('Read File') {
            steps {
             script {
              def fileContent = readFile 'README.md'
              echo(fileContent)
              def rootDir = pwd()
                println("Current Directory: " + rootDir)

                // point to exact source file
              def example = load "${rootDir}/Example.Groovy"
                example.exampleMethod()
                example.otherExampleMethod()
              }
              sh "printenv"
                echo "${GIT_URL}"
                echo GIT_URL.substring(GIT_URL.lastIndexOf('/')+1, GIT_URL.lastIndexOf('.'))
              dir("${GIT_URL}".substring("${GIT_URL}".lastIndexOf("/")+1, "${GIT_URL}".lastIndexOf("."))){   
                  sh "pwd"
                }
                sh "pwd"
                
               sh "ls -ltr"
              sh "cat README.md"
            }
        }
    }
}
