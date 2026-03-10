pipeline {
  agent any

  stages {

    stage('Clone') {
      steps {
        git url: 'https://github.com/vvce23ise0171-a11y/dev.git',
            branch: 'main'
      }
    }

    stage('Run Python Script') {
      steps {
        sh 'python3 --version'   // optional check
        sh 'python3 python.py'   // runs your python file
      }
    }
    stage('Run Python1 Script') {
      steps {
        sh 'python3 --version'   // optional check
        sh 'python3 bin.py'   // runs your python file
      }
    }

    stage('Run Script') {
      steps {
        sh 'chmod +x script.sh'
        sh './script.sh'
      }
    }
  }
}
