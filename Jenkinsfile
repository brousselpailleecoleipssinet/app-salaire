node{
 stage('Clone') {
 git 'https://github.com/brousselpailleecoleipssinet/app-salaire.git'
 }
 stage('Ansible') {
 ansiblePlaybook (
 colorized: true, 
 become: true, 
 playbook: 'install-able.yaml',
 inventory: 'hosts.yaml'
 )
 }
}
