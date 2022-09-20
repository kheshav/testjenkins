pipeline {
  agent any
  environment {
    DISABLE_AUTH = 'true'
    DB_ENGINE = 'sqlite'
  }
  parameters{
    string(name: "TEST_STRING", defaultValue: "t", trim: true, description: "THis is test string")
  }
  stages {
    stage('build') {
      steps {
        echo "Database engine is ${DB_ENGINE}"
        echo "DISABLE_AUTH is ${DISABLE_AUTH}"
        echo "Test string is $params.TEST_STRING"
        sh 'printenv'
       }
     }
  }
}
