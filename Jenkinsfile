node {

stage('delet ws')
	{
	cleanWs()	
	}
	
	
    
 stage('Git checkout'){
	git 'https://github.com/joshiPriya/hello-world.git'
}

stage('compile-package')
{
    def mvnhome = tool name: 'maven3', type: 'maven'
    sh "${mvnhome}/bin/mvn clean package"

}
 /*
  stage('SSh-connection'){
        sshPublisher(publishers: [sshPublisherDesc(configName: 'docker-host', transfers: [sshTransfer(cleanRemote: false, excludes: '', execCommand: 'docker stop mywebapp1; docker rm -f mywebapp1; docker image rm -f mywebapp1; docker image rm -f prijo1/mywebapp1:v1; cd /home/dockeradmin/docker;docker build -t mywebapp1 .;docker tag mywebapp1 prijo1/mywebapp1:v1;docker push prijo1/mywebapp1:v1', execTimeout: 120000, flatten: false, makeEmptyDirs: false, noDefaultExcludes: false, patternSeparator: '[, ]+', remoteDirectory: '//home//dockeradmin//docker', remoteDirectorySDF: false, removePrefix: 'webapp/target', sourceFiles: 'webapp/target/*.war')], usePromotionTimestamp: false, useWorkspaceInPromotion: false, verbose: true)])

    
 } */


}
