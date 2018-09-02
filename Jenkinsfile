pipeline {
    agent any

    stages {
        stage('Master') {
            steps {
				git checkout test
				git merge master
				git commit -test
            }
        }
        stage('Test') {
            steps {
               git checkout master
			   git merge test
			   git commit -master
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}