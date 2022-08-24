pipeline {
  agent any
  Parameter{
    File Parameter 'file_path'
  }
    
  stages {
      stage ("build"){
          steps{
            echo "Build success"
            WithFileParameter ('file_path')
            sh 'cat $file_path'
           }
      }
  }
}
