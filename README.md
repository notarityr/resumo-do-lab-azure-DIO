# resumo-do-lab-azure-DIO
 Resumo de aprendizado do Bootcamp "Microsoft 50 Anos - Computação em Nuvem com Azure" da atividade do Lab "Microsoft Azure - Localizando Serviços por Categoria".

## ⚡Computação em Nuvem
<p style="text-align: justify;">A computação em nuvem é um modelo de fornecimento de serviços de tecnologia em que recursos como armazenamento, processamento, software e redes são disponibilizados pela internet, em vez de estarem localizados em servidores próprios. Esse modelo permite que empresas e usuários acessem esses serviços conforme a demanda, pagando apenas pelo que utilizam. Com isso, elimina-se a necessidade de investir em infraestrutura física cara e complexa de manter. A nuvem oferece escalabilidade, flexibilidade e rapidez, além de permitir o acesso remoto aos recursos, a qualquer hora e de qualquer lugar.</p>

## ⚡Tipos de Infraestrutura

### 📌On-Premise (Infraestrutura Local)
<p style="text-align: justify;">O modelo on-premise se refere à utilização de infraestrutura física e sistemas de TI instalados diretamente nas dependências da empresa, ou seja, em seu próprio data center. Nesse formato, toda a gestão dos dados e operações fica sob responsabilidade total da organização, que precisa adquirir, manter e operar servidores, softwares, redes e demais recursos tecnológicos. Embora proporcione um nível elevado de controle e segurança esse modelo demanda altos investimentos iniciais em equipamentos, espaço físico e equipe técnica especializada.</p>

👍Vantagens: Controle total sobre os dados, software, hardware e possibilidade de maior personalização.
<br>
<br>
👎Desvantagens: Elevados custos de manutenção, necessidade de equipe especializada e necessidade de estrutura física dedicada.

### 📌Modelo Cloud (na Nuvem)
<p style="text-align: justify;">O modelo cloud, ou de computação em nuvem, consiste em uma infraestrutura acessada via internet, onde empresas e usuários utilizam recursos de TI fornecidos por terceiros. Em vez de manter servidores, bancos de dados e sistemas internamente, as organizações contratam esses serviços de provedores como Amazon Web Services (AWS), Microsoft Azure, Google Cloud, entre outros. Essa abordagem permite ajustar a capacidade dos serviços conforme a demanda, sem a necessidade de investir em infraestrutura própria. Além disso, proporciona redução de custos, maior agilidade e acesso a tecnologias avançadas que seriam complexas ou caras de implementar localmente.</p>

👍Vantagens: Redução de custos, escalabilidade e maior flexibilidade.
<br>
<br>
👎Desvantagens: Dependência da conexão com a internet, dependência de fornecedores e suporte, segurança de dados sensíveis.

### 📌Modelo Híbrido (Hybrid)
<p style="text-align: justify;">O modelo híbrido integra as vantagens das abordagens on-premise e cloud, permitindo que a empresa utilize tanto infraestrutura local quanto serviços de nuvem. Nesse formato, parte dos sistemas e dados permanece nas instalações da organização, enquanto outras funções são executadas na nuvem. Por exemplo, é possível manter informações sensíveis em servidores próprios e utilizar a nuvem para aplicativos que demandam maior escalabilidade. Essa combinação proporciona flexibilidade para adaptar a infraestrutura às necessidades específicas de cada operação. Por outro lado, a gestão se torna mais complexa, já que é necessário coordenar e monitorar ambientes distintos.</p>

👍Vantagens: Flexibilidade para distribuir recursos conforme a necessidade, maior controle sobre dados e escalabilidade.
<br>
<br>
👎Desvantagens: Maior complexidade na administração e integração entre sistemas locais e da nuvem.

## ⚡Modelos de Serviços em Nuvem

### 📌Iaas (Infraestructure as a Service)

<p style="text-align: justify;">IaaS é um modelo de computação em nuvem que fornece infraestrutura de TI básica como serviço, incluindo servidores virtuais, armazenamento, redes e outros recursos essenciais. Os usuários pagam conforme o uso, sem a necessidade de investir em hardware físico.</p>

Exemplos:

- Microsoft Azure VMs
- Amazon EC2
- Amazon S3 
- Google Compute Engine
- Google Cloud Storage

👍Vantagens: Maior controle sobre a infraestrutura, com escalabilidade e flexibilidade.
<br>
<br>
👎Desvantagens: Exige configuração e gerenciamento dos servidores, implicando mais responsabilidades em comparação com os modelos PaaS ou SaaS.

### 📌PaaS (Platform as a Service)
<p style="text-align: justify;">PaaS é um modelo de computação em nuvem que fornece uma plataforma completa para o desenvolvimento de aplicativos, permitindo que os desenvolvedores criem, testem e implantem soluções sem se preocupar com a gestão de infraestrutura.</p>

Exemplos:

- Microsoft Azure App Services
- Google App Engine
- Google Cloud SQL
- Amazon RDS
- AWS Elastic Beanstalk

👍Vantagens: Facilita o desenvolvimento por não necessitar de infraestrutura local, permitindo foco total no código e na funcionalidade do aplicativo.
<br>
<br>
👎Desvantagens: Menor controle sobre a infraestrutura e restrições em customizações avançadas.

### 📌SaaS (Software as a Service)
<p style="text-align: justify;">SaaS é um modelo de serviço em nuvem que disponibiliza softwares e aplicações prontas para uso, acessíveis pela internet, sem necessidade de instalação local. Toda a infraestrutura, manutenção e atualizações ficam sob responsabilidade do provedor.</p>

Exemplos:

- Microsoft Office 365
- Google Workspace
- Zoom

👍Vantagens: Implantação rápida, sem necessidade de gerenciar infraestrutura, com pagamento baseado na utilização.
<br>
<br>
👎Desvantagens: Requer conexão com a internet e oferece menor controle sobre o software e os dados.

## ⚡Componentes de arquitetura do Azure

### 📌Regiões (Regions)
<p style="text-align: justify;">As regiões do Azure são conjuntos geográficos que contêm pelo menos um data center. Cada região é independente e oferece serviços de nuvem com baixa latência para usuários próximos.</p>

Exemplos: 

- East US
- West Europe
- Brazil South

As regiões são essenciais para localização de dados, conformidade e velocidade de transferência.

### 📌Zonas de Disponibilidade (Availability Zones)
<p style="text-align: justify;">Cada região pode conter múltiplas zonas de disponibilidade, que são localizações físicas separadas dentro da região. Cada zona tem sua própria energia, refrigeração e rede e são projetadas para oferecer alta disponibilidade e tolerância a falhas, permitindo a replicação de recursos entre as zonas.</p>

### 📌Pares de Regiões (Region Pairs)
<p style="text-align: justify;">O Azure organiza regiões em pares dentro da mesma área geográfica para garantir recuperação de desastres (DR) e resiliência geográfica. Os dados replicados entre pares têm prioridade na recuperação.</p>

Exemplo: Brazil South ↔️ South Central US

### 📌Regiões Soberanas (Sovereign Regions)
<p style="text-align: justify;">São regiões isoladas, criadas para atender requisitos regulatórios e de conformidade específicos de certos países, como por exemplo serviços Militares e Governamentais, com a localização de sua infraestrutura sendo desconhecida.

- Azure Government (EUA): voltado para agências governamentais dos EUA, com acesso restrito e alto nível de conformidade (como FedRAMP).

- Azure China: operado por um parceiro local (21Vianet), separado do restante da infraestrutura global da Microsoft, para cumprir leis e políticas locais.</p>

## ⚡Computação e rede do Azure
### 📌Recursos (Resources)
<p style="text-align: justify;">No Azure, recursos são as unidades básicas de serviço, como máquinas virtuais, bancos de dados, redes virtuais e contas de armazenamento.Os recursos são organizados em grupos de recursos (resource groups), que facilitam o gerenciamento, controle de acesso, e automação. Eles são configuráveis, escaláveis e muitas vezes integrados com monitoramento, segurança e políticas de governança.</p>

### 📌Serviços de Computação no Azure
<p style="text-align: justify;">Os serviços de computação do Azure permitem executar aplicativos, hospedar servidores e processar cargas de trabalho na nuvem, permitindo escalabilidade e flexibilidade.</p>

- Azure Virtual Machines (VMs):
Máquinas virtuais configuráveis na nuvem, ideais para aplicações legadas, hospedagem de servidores, testes e desenvolvimento.

 - Azure App Service:
Plataforma para hospedagem de aplicações web, APIs e back-ends móveis, com suporte a linguagens como .NET, Java, Node.js, Python e PHP.

- Azure Functions:
Serviço de computação serverless baseado em eventos que executa pequenos blocos de código sob demanda, sem se preocupar com a infraestrutura.

- Azure Batch:
Executa tarefas em paralelo e em grande escala usando pools de VMs, ideal para renderização, simulações e cálculos intensivos.

### 📌Serviços de Contêineres no Azure
<p style="text-align: justify;">Os serviços de contêineres permitem empacotar, executar e escalar aplicações de forma portátil e leve, usando tecnologias como Docker e Kubernetes.</p>

- Azure Container Instances (ACI)
Executa contêineres de forma rápida e isolada, sem necessidade de gerenciar VMs, sendo ideal para workloads curtos, scripts, microsserviços e testes.
- Azure Kubernetes Service (AKS)
Serviço gerenciado de orquestração de contêineres com Kubernetes, sendo possível automatizar atualizações assim como escalonamento e monitoramento de clusters.
- Azure Container Apps
Plataforma serverless para contêineres, focada em microsserviços e funções orientadas a eventos com Escala automática com base na demanda.

## ⚡Armazenamento do Azure

<p style="text-align: justify;">O Azure oferece uma infraestrutura de armazenamento escalável, com suporte a diferentes tipos de dados: arquivos, blobs, discos, filas, tabelas e bancos de dados.</p>

### 📌Redundância de Armazenamento (Storage Redundancy)
Para garantir a alta disponibilidade e durabilidade dos dados, o Azure oferece diferentes níveis de replicação:

Tipo de Redundância:
- LRS (Locally Redundant Storage): Replica os dados 3 vezes dentro do mesmo datacenter sendo mais econômico mas menos resiliente.
- ZRS (Zone-Redundant Storage):	Replica os dados em 3 zonas de disponibilidade dentro da mesma região oferecendo alta disponibilidade.
- GRS (Geo-Redundant Storage): Replica os dados para uma região secundária distante, além da replicação local (LRS).
- GZRS (Geo-Zone-Redundant Storage): Combina ZRS com GRS oferecendo alta disponibilidade local e replicação geográfica.


### 📌Serviços de Armazenamento no Azure
O Azure Storage oferece vários serviços especializados, cada um para tipos de dados e usos diferentes:

- Blob Storage: Armazenamento de objetos (imagens, vídeos, backups, logs etc.).
- File Storage (Azure Files):	Compartilhamento de arquivos via SMB (como um drive de rede).
- Disk Storage: Discos gerenciados para máquinas virtuais.
- Queue Storage: Fila de mensagens para comunicação entre componentes distribuídos.
- Table Storage: Armazenamento NoSQL para dados estruturados.

### 📌Pontos de Extremidade (Endpoints)
<p style="text-align: justify;">Cada conta de armazenamento possui pontos de extremidade únicos para acessar seus serviços via HTTP/HTTPS, variando de acordo com o serviço (Blob, File, Queue, Table)</p>

Exemplos de endpoints:

https://nomedaconta.blob.core.windows.net (Blob Storage)

https://nomedaconta.file.core.windows.net (File Storage)

### 📌Azure Data Box
<p style="text-align: justify;">O Azure Data Box é uma solução física usada para migrar grandes volumes de dados para o Azure, ideal quando a transferência por internet é impraticável. A Microsoft envia o dispositivo ao cliente que copia os dados localmente e devolve o dispositivo e carregados à cloud pela Microsoft.</p>

