@Library('Pipeline-shared-scripts') _
pipeline {
agent any
tools {nodejs "node"}
stages {
stage('build') {
steps {
sh 'npm install'
sh 'npm --version'
script{
def res = standardHeaderValidator("xyz");
println("FinalResult: ${res}")
}
}
}
}
}