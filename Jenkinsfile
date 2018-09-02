pipeline {
    agent any

    stages {
        stage('Master') {
            steps {
				bat "git checkout test"
				bat "git merge origin/master"
				bat "git commit -test"
            }
        }
        stage('Test') {
            steps {
               bat "git checkout master"
			   bat "git merge origin/test"
			   bat "git commit -master"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}