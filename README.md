# DIOlab1
Laboratório EC2-DIO

Laboratório EC2
•	Desenvolvedor externo acessa via Systems Manager Session Manager uma instância EC2 na AWS, garantindo acesso seguro ao ambiente Cloud.
•	Há AMI já desenvolvida para essa instância, garantindo que o desenvolvedor não se preocupe com o ambiente, apenas em seu fluxo de trabalho.
•	Para o armazenamento utilizamos o EBS, com Snapshots, o serviço funciona como um disco rígido para instância, oferecendo persistência de dados. Os snapshots garantem o recovery de dados, facilitando a recuperação e replicação deles.
•	O Backup é armazenado em um S3, naturalmente os snapshots são enviados ao S3, o que garante a integridade dos dados, já que o EBS é atachado diretamente a instância.
