pipeline {
    agent any

    stages {
        stage('Test Branch') {
            steps {
               bat "git checkout master"
			   bat "git merge origin/test"
			   bat "git commit -master"
            }
        }
		stage('Nigam Branch') {
            steps {
               bat "git checkout master"
			   bat "git merge origin/nigam"
			   bat "git commit -master"
            }
        }
    }
}