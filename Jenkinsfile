pipeline {
  agent any
  stages {
    stage('dependencies') {
      steps {
        echo 'dependencies'
      }
    }
    stage('build') {
      steps {
        echo 'build'
      }
    }
    stage('testing-phase') {
      parallel {
        stage('unit-test') {
          steps {
            echo 'unit-test'
          }
        }
        stage('integration-test') {
          steps {
            echo 'integration-test'
          }
        }
        stage('static-code-analysis') {
          steps {
            echo 'static code analysis'
          }
        }
        stage('performance-test') {
          steps {
            echo 'performance test'
          }
        }
      }
    }
    stage('package') {
      steps {
        echo 'package'
      }
    }
    stage('deploy') {
      steps {
        echo 'deploy'
      }
    }
    stage('functional-test') {
      steps {
        echo 'functional-test'
      }
    }
    stage('notify') {
      steps {
        echo 'notify'
      }
    }
  }
}