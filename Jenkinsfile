pipeline{
  agent any;
  stages {
    stage ('BUILD') {
      steps {
        echo "this is build stage"
      }
   }

    stage ('Test in parallel') {
    parallel {
      stage ('TEST 1') {
        steps {
          echo " test 1 in parallel"
     }
    }
      stage ('TEST 2') {
        steps {
          echo "test 2 in parallel"
        }
      }
    }
  }
 }
}
