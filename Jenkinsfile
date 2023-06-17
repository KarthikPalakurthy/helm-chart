pipeline {

    agent any

    parameters {

        string(name: 'COMPONENT', defaultValue: '', description: 'Component name')
        string(name: 'COMPONENT', defaultValue: '', description: 'App version')
    }

    stages {

      stage('Get Values file') {
            steps {
                dir('APP') {
                    git branch: 'main', url: 'https://github.com/KarthikPalakurthy/${COMPONENT}.git'
                }
            }
      }

      stage('Helm Deployment') {
            steps {
                sh 'find .'
            }
      }
    }
}
