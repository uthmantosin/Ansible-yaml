pipeline{
  agent any  
  stages{  
      stage("Run ansible playbook"){
        steps{
        ansiblePlaybook credentialsId: 'ssh-key', inventory: 'hosts', playbook: 'nginx_install.yaml', vaultTmpPath: ''
        
        }
      }
  }
}
