pipeline 
{
    agent any

    stages 
	{
        stage('Developer') 
		{
            steps 
			{
			   bat "git pull origin master"
			   bat "git checkout test"
			   bat "git merge master"
			   bat "git commit -origin/test"
			   echo("Developer Code is updated")
            }
        }
		stage('Nigam Branch') 
		{
            steps 
			{
               bat "git pull origin test"
			   bat "git checkout nigam"
			   bat "git merge test"
			   bat "git commit -origin/nigam"
            }
        }
		stage('Master Branch') 
		{
            steps 
			{
               bat "git pull origin nigam"
			   bat "git checkout master"
			   bat "git merge nigam"
			   bat "git commit -origin/master"
            }
        }
    }
}