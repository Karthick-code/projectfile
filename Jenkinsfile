pipeline {
  agent any
  Parameters{
    FileParameter 'newtext.txt'
  }
    
  stages {
      stage ("build"){
          steps{
              echo "Build success"
           }
      }
      stage("upload") {
          steps{
              WithFileParameter ('newtext.txt')
              sh 'cat $newtext.txt'
        ` }
      }
    }
}
