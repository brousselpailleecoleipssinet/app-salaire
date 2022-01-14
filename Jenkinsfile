node{
 stage('Clone') {
 git 'https://github.com/brousselpailleecoleipssinet/app-salaire.git'
 }
 stage('Ansible') {
 ansiblePlaybook (
 colorized: true, 
 become: true, 
 playbook: 'playbook.yml',
 inventory: 'hosts.yml'
 )
 }
}
