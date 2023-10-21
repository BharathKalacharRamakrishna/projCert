pipeline {
    agent {
    label "WORKER"
    }
    stages {
	stage('Install Puppet') {
	    steps{
		sh ''' 
		    pwd
		    cd /home/ubuntu
		    pwd
		    wget https://apt.puppetlabs.com/puppet6-release-focal.deb
		    sudo dpkg -i puppet6-release-focal.deb
		    sudo apt-get update -y
		    sudo apt-get install puppet-agent -y
		    '''
	    }
	}
    }
}

