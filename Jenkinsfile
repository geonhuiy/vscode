pipeline {
  agent any /*{
    kubernetes {
      label 'geonhuiy-vscode'
      yaml """
      apiVersion: v1
      kind: Pod
      spec:
        containers:
          - name: test-nginx
          - image: nginx
      """
    }
  }*/
  stages {

    stage('Build') {
      steps {
        echo 'Build'
      }
    }
    stage('Test') {
      steps {
        container('test-nginx') {
          echo 'Test'
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy'
      }

    }
  }
}
