@Library('piper-lib-os') _

node() {
  stage('init') {
    deleteDir()
    checkout scm
  }
 stage('integrationArtifactUpdateConfiguration Command') {
	  	 setupCommonPipelineEnvironment script: this
		integrationArtifactGetMplStatus script: this
	  	print "status:" 
	  	print  commonPipelineEnvironment.getValue("iFlowMplStatus")
  }
}
