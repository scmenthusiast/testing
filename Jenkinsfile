node("master")
{
    stage("Git Checkout") 
    {
	checkout([
		$class: 'GitSCM', 
		branches: [[name: '*/*']], 
		gitTool: 'Default', 
		userRemoteConfigs: [
			[
				credentialsId: 'prasadve', 
				url: 'git@github.com:scmenthusiast/testing.git'
			]
		]
	])
    }
	
    stage("Plugin Package")
    {
        sh '''
		echo "Hello World!"	
        '''
    }

}
