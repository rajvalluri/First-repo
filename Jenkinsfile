pipeline {
  agent any
  stages {
    stage('phase1') {
      steps {
        echo 'hello phase1'
      }
    }
    stage('phase2') {
      steps {
        parallel(
          "phase2": {
            echo 'phase2'
            
          },
          "parallel1": {
            echo 'parallel1'
            
          },
          "Parallel2": {
            echo 'parallel2 phase'
            
          },
          "phase3": {
            echo 'parallel phase 3'
            
          }
        )
      }
    }
    stage('finalphase') {
      steps {
        echo 'phase finished'
      }
    }
  }
}