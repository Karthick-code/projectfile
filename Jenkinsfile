pipeline {
  agent any
  Parameter{
    FileParameter 'newtext.txt'
  }
    
  stages {
      stage ("build"){
          steps{
            echo "Build success"
            WithFileParameter ('newtext.txt')
            sh 'cat $newtext.txt'
           }
      }
    stage("upload") {
        def inputFile = input message: 'Upload file', parameters: [file(name: "$/home/karthi/Documentation/newtext.txt")]
        }
  }
}
