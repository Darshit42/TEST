pipeline
{
    agent any 
    tools {
        maven 'maven'
    }
    stages {
        stage('Build') {
            steps {
                sh ('git clone https://github.com/Darshit42/TEST.git')
                sh ('npm install')
            }
        }
        stage('Test') {
            steps {
                sh('npm test')
            }
        }
        stage('Run'){
            steps{
                sh ('npm run build')
            }
        }
        
    }
}
