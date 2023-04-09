pipeline {
	agent any
    stages {
        stage('Build on k8s ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/bin/helm upgrade --install petclinic-app petclinic  --set image.repository=docker.io/pramodpra/petclinic --set image.tag=1'
              			
            }           
        }
    }
}