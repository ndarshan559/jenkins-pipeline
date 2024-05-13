pipeline{
  agent any;
  parameters {
  string defaultValue: 'TEST', description: 'environment to deploy application', name: 'ENV', trim: true
}
  stages {
    stage ('BUILD') {
      steps {
        echo "this is build stage $params.ENV"
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
