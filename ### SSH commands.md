### SSH commands

- ssh -i <arquivo> <sistema>@<ip da maquina>
<!-- EX: ssh -i id_rsa.pub vagrant@192.168.1.1 -->
<!-- Se conecta a uma maquina virtual, passando o arquivo com a chave ssh (-i) -->
<!-- e tambem passando o sistema operacional rodando + o ip -->
<!-- EX2: ssh -i public_key.pub ubuntu@192.168.0.1 -->

- ssh-keygen -t rsa
<!-- cria uma chave ssh -->