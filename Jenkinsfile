pipeline
{
    agent any 
    tools {
        maven 'maven'
    }
    stages {
        stage('Build') {
            steps {
                sh ('npm install')
            }
        }
        stage('Test') {
            steps {
                sh('npm test')
            }
        }
        stage('Build'){
            steps{
                sh ('npm run build')
            }
        }
        
    }
}
