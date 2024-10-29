# desafio-da-DIO
Neste guia, vou compartilhar meu aprendizado sobre como criar máquinas virtuais no Azure, detalhando os passos que segui durante o desafio DIO. O objetivo é fornecer um passo a passo prático e personalizado, com base na minha experiência.

Conceitos-chave

Máquina Virtual (VM): Um computador virtualizado que roda em um servidor físico.
Grupo de recursos: Um contêiner lógico para organizar e gerenciar seus recursos do Azure.
Região: A localização geográfica dos seus recursos.
Zona de disponibilidade: Uma subdivisão de uma região para alta disponibilidade.
Conjunto de dimensionamento: Um grupo de VMs idênticas que podem ser escaladas automaticamente.
Disco: O armazenamento para sua VM.
Rede virtual: Uma rede isolada dentro do Azure.
Sub-rede: Uma divisão lógica de uma rede virtual.
Grupo de segurança de rede (NSG): Uma lista de regras de segurança que filtra o tráfego de rede para suas VMs.
Passo a passo para criar uma máquina virtual (detalhes do meu desafio)

Criar um grupo de recursos:

No portal do Azure: Naveguei até a seção "Grupos de recursos" e cliquei em "Criar".
Nomeei o grupo de recursos: "AZ-900_Lab_DIO_VM".
Selecionei a região: "East US 2".
Cliquei em "Criar".
Criar uma máquina virtual:

Cliquei em "Criar um recurso" e pesquisei por "Máquina virtual".
Selecionei a imagem: "Ubuntu Server 22.04 LTS". Escolhi o Ubuntu por ser um sistema operacional Linux popular e gratuito.
Configurei o tamanho: Escolhi o tamanho "Standard_B2s". Considerando que o desafio não exigia alta performance, esse tamanho foi suficiente para minhas necessidades.
Criei uma nova rede virtual: Nomeei a rede virtual como "VNet_DIO" e a sub-rede como "Subnet_DIO". Isso permitiu isolar minha máquina virtual e controlar o fluxo de tráfego.
Configurei o disco: Escolhi um disco SSD de 30 GB. Optei por um SSD devido à sua maior velocidade de leitura e escrita.
Configurei as regras de NSG: Permiti o acesso SSH (porta 22) para gerenciar a máquina remotamente e o acesso HTTP (porta 80) para futuras aplicações web.
Cliquei em "Revisar e criar" e depois em "Criar".
Observações:

Escolhi o Ubuntu Server 22.04 LTS por ser um sistema operacional estável e amplamente utilizado.
O tamanho Standard_B2s atendeu às minhas necessidades, oferecendo um bom equilíbrio entre custo e desempenho.
Criei uma nova rede virtual e sub-rede para garantir o isolamento e controle do tráfego da minha máquina virtual.
Permiti apenas o acesso SSH e HTTP para fortalecer a segurança da minha máquina.

Falamos sobre:

Tipos de máquinas virtuais
Recursos adicionais
Best practices

Nesta primeira parte do guia, detalhei os passos que segui para criar minha primeira máquina virtual no Azure durante o desafio DIO. Nas próximas seções, explorarei outros aspectos importantes, como os diferentes tipos de máquinas virtuais, recursos adicionais e melhores práticas.

Com este guia, espero que você possa criar suas próprias máquinas virtuais no Azure de forma eficiente e segura.

Próximos passos:

Configurar o DNS: Associar um nome de domínio à sua máquina virtual.
Integrar com outros serviços do Azure: Conectar sua máquina virtual a outros serviços, como bancos de dados e serviços de armazenamento.
Automatizar a criação de máquinas virtuais: Utilizar scripts PowerShell ou Azure CLI para automatizar o processo.
Gerenciar custos: Aprender a otimizar os custos das suas máquinas virtuais.



