pipeline {
  agent none
  stages {
    stage('Build') {
      agent {
        docker {
          image 'test_python'
        }

      }
      steps {
        sh 'python -m py_compile sources/add2vals.py sources/calc.py'
      }
    }

  }
}