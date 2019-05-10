pipeline
{
  agent any
  stages
    {
      stage('one')
      {
      steps {
      echo 'hi , HELLO WORLD!!!'
      }
      }
      stage('two')
      {
      steps {
      input('Do you wish to proceed ?')}
      }
      stage('three')
      {
      parallel {
        stage('UT') {
            steps { 
                echo 'UNIT TESTING' }
          } 
      stage('IT') {
          steps {
              echo 'INTEGRATION TESTING' }
              }
    }
}
