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
  
}
