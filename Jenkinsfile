pipeline 
{
    agent any

    stages 
	{
        stage('Developer') 
		{
            steps 
			{
			  bat "ant -version"
			  // bat "git pull origin master"
			  // bat "git checkout test"
			  // bat "git merge master"
			  // bat "git commit -m 'aa'"
			  // bat "git push origin test"
			  // echo("Developer Code is updated")
            }
        }
		stage('Nigam Branch') 
		{
            steps 
			{
              // bat "git pull origin test"
			   //bat "git checkout nigam"
			   //bat "git merge test"
			   //bat "git commit -m 'aa'"
			   //bat "git push origin nigam"
            }
        }
		stage('Master Branch') 
		{
            steps 
			{
              // bat "git pull origin nigam"
			  // bat "git checkout master"
			  // bat "git merge nigam"
			   //bat "git commit -m 'aa'"
			   //bat "git push origin master"
            }
        }
    }
}