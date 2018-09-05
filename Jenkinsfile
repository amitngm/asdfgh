pipeline 
{
    agent any

    stages 
	{
        stage('Developer') 
		{
            steps 
			{
			  withAnt(installation: 'Ant-1.10.5') {
					bat "ant -version"
					echo("Developer Code is updated")
				}
			}
        }
    }
}