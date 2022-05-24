#!groovy?

pipeline {
	agent any 
	options {
        buildDiscarder(logRotator(numToKeepStr: '20', artifactNumToKeepStr: '30', daysToKeepStr: '15'))
        disableConcurrentBuilds()
    }

    tools {
    maven 'Maven 3.3.9'
    }

    environment {
        credentialsId = "ab6b02f9-6662-4428-ab47-34c0a18c560d"
        s3_bucket_region = "ap-southeast-1"
	    s3_profile_name = "BnD Packages"
    }

    /// Repositories

}
