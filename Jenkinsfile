node {
	stage('SCM Checkout') {
		git credentialsId: 'id1', url: 'https://github.com/edureka-devops/projCert'
	}
	stage('Mvn Package'){
	    sh 'mvn clean package'
	}
	stage('Buidl Docker Image'){
	    sh 'docker build -t naren27/php:2.0.0 .'
	}

}
