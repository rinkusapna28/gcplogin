pipeline{
    agent any
	stages{
	    stage ('login GCP'){
	         steps {
	        sh 'gcloud auth activate-service-account vmcreate@studied-point-232906.iam.gserviceaccount.com --key-file=studied-point-232906-73b79b66139a.json --project=studied-point-232906'
	        } 
	    }
	   stage ('creation of topics'){
	         steps {
	        sh 'gcloud compute instances create example-instance --image-family=ubuntu-minimal-1604-lts --image-project=ubuntu-os-cloud --zone=us-central1-a'
	        } 
	    } 
	
	}
}
