
node () {	
    	stage ('checkout'){
	echo "checkout "
	checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/csenapati12/antrepo.git']]]
	}
	
	stage ('ant Build'){
	 bat """
	 set path=%path%;C:\\Program Files\\Java\\jdk1.8.0_191\\bin
	 ant 
	"""
	}

		stage ('Email Notification') {
		   
		echo "email"
	} 

	
	
}
