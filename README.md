# Criação de máquina virtual Amazon Linux - EC2 AWS

Esse projeto, desenvolvido como parte do curso Arquitetos de Nuvem AWS, da Proz Educação, aborda a necessidade da banda de Miguel em organizar e gerenciar sua documentação e arquivos importantes na nuvem. Para isso, foi necessário criar uma instância EC2 na AWS, utilizando o Amazon Linux 2, uma distribuição otimizada para ambientes de nuvem. A solução foi projetada para oferecer à banda uma infraestrutura eficiente e escalável, garantindo o armazenamento seguro e o fácil acesso aos seus arquivos na nuvem.

Entre os principais benefícios do Amazon EC2, estão:

* **Escalabilidade:** O Amazon EC2 permite que o cliente inicie, pare, acesse e dimensione instâncias de servidores virtuais de maneira simples e rápida. Com uma ampla variedade de tipos de instância e tamanhos, é possível escolher a configuração mais adequada para as necessidades de computação e ajustar recursos com base na demanda, utilizando serviços como Auto Scaling para otimizar a performance e os custos.

* **Custo sob Ddmanda:** O EC2 adota um modelo de pagamento por uso, permitindo que o cliente pague apenas pelos recursos de computação que consome. Isso elimina a necessidade de investimentos iniciais em hardware e infraestrutura, além de permitir a escolha entre diferentes opções de preço, como instâncias reservadas, spot, para obter descontos em função do tempo de uso e da flexibilidade.

* **Alta disponibilidade e confiabilidade:** O EC2 oferece uma infraestrutura robusta, com zonas de disponibilidade distribuídas globalmente, garantindo alta disponibilidade e continuidade dos serviços. Através da utilização de instâncias distribuídas em diferentes zonas e regiões, o cliente pode configurar sistemas de recuperação automática, tornando as aplicações mais resilientes a falhas e interrupções.



## Configuração

1 - Exemplo de criação de uma instância EC2:
![images](https://github.com/phatima05/proz-ec2-aws/blob/main/images/Amazon%20Linux%201.png)

![images](https://github.com/phatima05/proz-ec2-aws/blob/main/images/Amazon%20Linux%202.png)

* Instância concluída:
![images](https://github.com/phatima05/proz-ec2-aws/blob/main/images/Amazon%20Linux%203.png)


2 - Acessando a instância Amazon Linux via SSH:
![images](https://github.com/phatima05/proz-ec2-aws/blob/main/images/EC2%20SSH.png)


3 - Criação de um volume EBS (EBS Teste):
![images](https://github.com/phatima05/proz-ec2-aws/blob/main/images/EBS.png)


* Volume **EBS Teste** alocado à instância **EC2 Proz** (xvdbb):

![images](https://github.com/phatima05/proz-ec2-aws/blob/main/images/EBS%20alocado.png)


4 - Montagem de volume:

![images](https://github.com/phatima05/proz-ec2-aws/blob/main/images/Montagem%20EBS.png)

![images](https://github.com/phatima05/proz-ec2-aws/blob/main/images/Volume%20montado.png)

* O comando **sudo mkdir /mnt/ebs-teste** cria um diretório para montar o volume

* O comando **sudo mount /dev/xvdbb /mnt/ebs-teste** monta um volume **xvdbb** no diretório recém-criado


5 - Um arquivo chamado **proz.txt**, com a nota **Proz Educação** foi criado:

![images](https://github.com/phatima05/proz-ec2-aws/blob/main/images/Arquivo%20criado%20no%20diret%C3%B3rio.png)


