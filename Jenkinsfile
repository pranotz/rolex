pipeline {
	agent any 
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/pranotz/Documents/Devops_software/apache-tomcat-9.0.82/bin/mvn install'
	                 }}
		stage('Deployment'){
		   steps {
		sh 'cp target/rolex.war /home/pranotz/Documents/Devops_software/apache-tomcat-9.0.82/bin'
			}}	
}}
