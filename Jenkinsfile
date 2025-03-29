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
                sh('npm test' || echo'NO tests defined')
            }
        }
        stage('Build'){
            steps{
                sh ('npm run build')
            }
        }
        
    }
}


echo "# TEST" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/Darshit42/TEST.git
git push -u origin main