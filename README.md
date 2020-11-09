# APS2020-2
Repositório para Atividade Prática Supervisionada da Universidade Paulista para o segundo semestre de 2020.

Componentes do Grupo:
Gabriel Murakami - RA: D40CIH5 - Turma: CC8P12
Thais Moreira da Silva - RA: D397IA0 - Turma: CC8P12

Proposta: Desenvolvimento de um tutorial de utilização de algum serviço da AWS.

Trabalho desenvolvido: Tutorial - Criação de Máquina Virtual Linux na AWS. 

Instruções para conectar a máquina virtual Linux criada na AWS:

1. Fazer o download da chave para conexão via SSH que está nesse diretório, arquivo "key-ec2-aps2020.pem"

2. Após realizar o download da chave, coloque em um diretório de fácil acesso em seu dispositivo, em seguida abra o prompt de comando do seu computador e navegue até o diretório em que a chave está localizada, em seguida execute o seguinte comando:

ssh -i "key-ec2-aps2020.pem" ubuntu@ec2-18-189-188-181.us-east-2.compute.amazonaws.com

3. Ao executar o comando ele retornará com uma pergunta, se você tem certeza de que deseja continuar com a conexão, “Are you sure you want to continue connecting (yes/no)?” responda em seu prompt de comando “yes”. 

4. Prontinho, sua conexão com a máquina virtual Linux criada pelo projeto APS foi estabelecida.
