pipeline {
  agent any
  Parameter{
    FileParameter 'file_path'
  }
    
  stages {
      stage ("build"){
          steps{
            echo "Build success"
            WithFileParameter ('newtext.txt')
            sh 'cat $file_path'
           }
      }
    stage("upload") {
        def inputFile = input message: 'Upload file', parameters: [file(name: "$/home/karthi/Documentation/newtext.txt")]
        }
  }
}
