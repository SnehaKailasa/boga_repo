node {
	stage ('Checkout SCM') {
		//checkout([$class: 'GitSCM', branches: [[name: '*/branch1']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/boga5/boga_repo.git']]])	
		checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: '']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '', name: '', refspec: '', url: 'https://github.com/boga5/boga_repo.git']]]
	}
	
	stage ('Test Build') {
		sh '''./file.sh'''
	}
}
