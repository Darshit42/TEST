pipeline
{
    agent any 
    tools {
        maven 'maven'
    }
    stages {
        stage('Build') {
            steps {
                sh ('rm -rf TEST')
                sh ('git clone https://github.com/Darshit42/TEST.git')
                sh ('cd TEST')
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
                sh('npm run')
                sh ('node server.js')
                sh ('kill localhost:3000')
                sh ('npm run server.js')
                sh ('npm run build')
            }
        }
        
    }
}
