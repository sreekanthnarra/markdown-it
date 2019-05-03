##################
Local Setup Documentation
##################

1) Be sure to set up java_home or add java(jdk1.8) to your PATH variable.
2) Be sure your machine installed with JBOSS (jboss-eap-7.0.x - currently we have 7.0.4).
3) Clone/Download the project from GIT.
4) Configure the standalone.xml
	 Replace local C:\JBOSS\jboss-eap-7.0.4\standalone\configuration\standalone.xml file with file available at /build/localsetup/
5) Update DB username and password for RE, PrepRating and Connect-5 in standalone.xml in datasource modules
	##username##
	##password###	  
6) Configure JBoss modules 
		Follow steps from - 1. Modules in share path document.
	  	Share Point : http://teams.thehartford.com/project/jbossmigration/Project%20Documents/JBoss%20Documents/2-Pre-Arch%20Asmt/JBOSS%20Assessment/Middle%20Market%20%2B%20Specialty%20IT/CUE/Upgrade%20Related/Local%20Setup/CUE_JBOSS_Local_Setup.docx?Web=1
6) Build the project 
		Follow steps from - 2. Run the build in share path document.
7) Update the Jboss memory Parameters in C:\JBOSS\jboss-eap-7.0.4\bin\standalone.bat
	Refer to point -3 in share path document
8) Deploy to JBoss after build success 
		a. copy /stage/CUERiskEval.ear file and paste C:\JBOSS\jboss-eap-7.0.4\standalone\deployments.
		b. open cmd and run standalone.bat
9) Run the DB synonyms. Follow steps from - 6.Run the DB synonyms - in share path document.
10) Launch Local application  http://localhost:8080/riskeval/ ,Enjoy!
