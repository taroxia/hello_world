pipeline {
  stage('prepare'){
    steps {
        sh 'mkdir -p build'
    }
  }

  stage('build'){
    steps {
      sh '''
        cd build &&
        cmake -D CMAKE_BUILD_TYPE=Debug -D BUILD_TESTING=ON .. &&
        make
      '''
    }
    // build...
  }

  stage('test'){
    // test...
  }
}
