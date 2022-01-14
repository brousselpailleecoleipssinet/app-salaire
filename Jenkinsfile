node{
 stage('Clone') {
 git 'https://github.com/brousselpailleecoleipssinet/app-salaire.git'
 }
 stage('Ansible') {
 ansiblePlaybook (
 colorized: true, 
 become: true, 
 playbook: 'install-table.yaml',
 inventory: 'hosts.yaml'
 )
 }
}
