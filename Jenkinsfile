pipeline {
  agent any
  stages {
    stage('') {
      steps {
        sh '''sudo apt -y update
sudo apt -y install python-pip virtualenv
virtualenv "${WORKSPACE}/venv"
source "${WORKSPACE}/venv/bin/activate"
pip install -r requirements.txt
python tests.py
'''
      }
    }
  }
}