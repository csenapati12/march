
node () {	
    	stage ('checkout'){
	echo "checkout "
	checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/csenapati12/antrepo.git']]]
	}
	
	stage ('ant Build'){
	sh label: '', script: 'ant'
		
	}

		stage ('Email Notification') {
		   
		echo "email"
	} 

	
	
}
