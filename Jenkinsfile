pipeline {
    agent any

    stages {
        stage('Master') {
            steps {
				bat "git checkout test"
				bat "git merge master"
				bat "git commit -test"
            }
        }
        stage('Test') {
            steps {
               bat "git checkout master"
			   bat "git merge test"
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