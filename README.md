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

3.1. Caso acontece um erro tipo: 
![alt text](https://i.imgur.com/PkcREiP.jpg)

Então faça o seguinte, entre no doretório onde está a sua chave "key-ec2-aps2020.pem", e entre nas propriedades dele. Depois vá até a aba "Segurança" e clique em "Avançadas":

![alt text](https://i.imgur.com/VwodYak.jpg)

Vá em "Desabilitar Herança" e clique em "Converter as permissões herdadas em permissões explícitas no objeto."

![alt text](https://i.imgur.com/aTDikwh.jpg)

Em seguida Remova todas as entradas de permissões, deixando apenas com a Entidade de segurança do seu Usuário: 

![alt text](https://i.imgur.com/zxNOLLg.jpg)

E por fim, Aplique as mudanças feitas e tente novamente.

4. Prontinho, sua conexão com a máquina virtual Linux criada pelo projeto APS foi estabelecida.
