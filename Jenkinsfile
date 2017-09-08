node 
{
        stage 'checkout'
       		checkout scm
	stage 'Build'
            	sh 'payslip/pom.xml', goals: 'clean install'
           
        stage 'Publish build info'
            server.publishBuildInfo buildInfo
            
            
}
