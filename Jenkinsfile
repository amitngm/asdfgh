pipeline 
{
    agent any

    stages 
	{
        stage('Test Branch') 
		{
            steps 
			{
               bat "git checkout master"
			   bat "git pull origin master"
			   bat "git merge test"
			   bat "git push origin master"
            }
        }
		stage('Nigam Branch') 
		{
            steps 
			{
               bat "git pull origin master"
			   bat "git merge origin/nigam"
			   bat "git push origin master"
            }
        }
    }
}