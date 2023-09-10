pipeline {
  /*
   * TODO: Implement pipeline stages/steps
   *   See documentation: https://www.jenkins.io/doc/book/pipeline/syntax/#stages
   */
  agent any 

  stages {
    stage('Checkout'){
      steps{
        // Checkout your source code from version control if needed
        // For example, you can use 'git checkout' here
        'git checkout'
        
      }
    }

    stage('Build'){
      steps{
        //Build project using ./gradlew assemble or the build command sh './gradlew assemble'
        sh './gradlew assemble'
      }
    }

    stage('Test'){
      steps{
        // run tests using ./gradlew test or test commadn sh './gradlew test'
        sh './gradlew test'
      }
    }

    // add more stages   
   }


  post{
    always{
      //perform cleanup / post-build actions here 
    }
  }
  
}
