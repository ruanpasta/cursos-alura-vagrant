### Vagrant commands

- vagrant list-commands
<!-- lista os comandos do vagrant -->

- vagrant init <box>
<!-- Este comando cria um Vagrantfile.
  
  ex: vagrant init hashicorp/precise64
  Inicia uma configuracao de ambiente pronta, buscando as informacoes da hashicorp.
  O comando precise64 da hashicorp cria uma maquina linux na versao 12lts 64bits
-->

- vagrant up <config>
<!-- roda a configuracao do arquivo Vagrantfile para criar a maquia virtual -->
<!-- EX: vagrant up -->
<!-- Tambem pode ser usada para rodar apenas a configuracao 
      de uma maquina do arquivo -->
<!-- EX: vagrant up mysqldb -->
<!-- EX: vagrant up phpweb -->

- vagrant status
<!-- mostra os status do maquina levantada -->

- vagrant global-status
<!-- mostra o status de todos os ambientes que existem na maquina -->

- vagrant halt
<!-- para a maquina virtual -->

- vagrant suspend
<!-- suspende a maquina virtual -->

- vagrant ssh
<!-- connecta na maquia virtual levantada -->
<!-- EX: vagrant ssh -->
<!-- EX: vagrant ssh mysqldb -->

- vagrant ssh-config
<!-- mostra as configuracoes do vagrant -->

- vagrant reload
<!-- Reinicia a maquina virtual com as novas configuracoes do Vagrantfile sem
precisar parar a maquina, porem em alguns casos pode nao funcionar -->

- vagrant destroy
<!-- destroi a maquina virtual, porem nao apaga o arquivo vagrantfile.
pode-se usar um "vagrant destroy -f" para forcar a destruicao -->
<!-- EX: vagrant destroy -f -->
<!-- Tambem pode ser usada para rodar apenas a configuracao 
      de uma maquina do arquivo -->
<!-- EX: vagrant destroy -f phpweb -->
<!-- EX: vagrant destroy -f mysqldb -->

- vagrant destroy <id>
- vagrant up <id>
- vagrant halt <id>
<!-- Destroy/Sobe/Para a VM rodando de qualquer lugar do PC atraves do ID dela -->

- vagrant provision
<!-- executa todas as configs do Vagrantfile .provision -->

- vagrant validate
<!-- valida se o arquivo do Vagrantfile nao tem erros -->

- vagrant box <subcomand>
<!-- EX: vagrant box list // Lista os box(maquinas virtuais criadas) (pode ter mais de uma maquina por box) -->
<!-- EX: vagrant box prune // Remove as box duplicadas -->
<!-- EX: vagrant box remove hashicorp/precise64 // Remove a box especificada -->