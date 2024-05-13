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
      stage ('TEST') {
        echo " test 1 in parallel"
    }
      stage ('BUILD') {
        echo "test 2 in parallel"
     }
    
   }
  }
 }
}
