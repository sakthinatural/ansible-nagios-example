pipeline {
    agent any

    
    stages {
        stage('Build') {
            steps {
               
                git 'https://github.com/sakthinatural/ansible-nagios-example.git'
                
                ansiblePlaybook credentialsId: 'root', installation: 'ansible', inventory: 'hosts', playbook: 'install/nagios.yml'
             
            }

            
        }
    }
}
