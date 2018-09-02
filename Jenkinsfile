pipeline {
    agent any

    stages {
        stage('Master Branch') {
            steps {
				bat "git checkout test"
				bat "git merge origin/master"
				bat "git commit -test"
            }
        }
        stage('Test Branch') {
            steps {
               bat "git checkout master"
			   bat "git merge test"
			   bat "git commit -master"
            }
        }
    }
}