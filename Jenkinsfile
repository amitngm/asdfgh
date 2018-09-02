pipeline 
{
    agent any

    stages 
	{
        stage('Test Branch') 
		{
            steps 
			{
               bat "git checkout origin/master"
			   bat "git merge origin/test"
			   bat "git commit -origin/master"
            }
        }
		stage('Nigam Branch') 
		{
            steps 
			{
               bat "git checkout origin/master"
			   bat "git merge origin/nigam"
			   bat "git commit -origin/master"
            }
        }
    }
}