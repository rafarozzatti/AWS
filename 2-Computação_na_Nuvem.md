# Amazon EC2 (Elastic Compute Cloud)

O **Amazon EC2** é um serviço de computação em nuvem que permite criar **servidores virtuais (instâncias)** sob demanda. Ele oferece uma alternativa mais flexível, rápida e econômica em comparação com a infraestrutura tradicional (on-premises).

Com o EC2, é possível:

- Criar servidores em poucos minutos.
- Aumentar ou reduzir a capacidade conforme a demanda.
- Pagar apenas pelo tempo em que a instância estiver em execução.
- Personalizar configurações de processamento, memória, armazenamento e rede.

> **Resumo:** O Amazon EC2 fornece capacidade computacional escalável na nuvem, eliminando a necessidade de comprar e manter servidores físicos.

---

# On-Premises x Amazon EC2

Ao planejar uma infraestrutura, é importante entender as diferenças entre utilizar servidores próprios e utilizar a nuvem.

| On-Premises | Amazon EC2 |
|-------------|------------|
| Compra de hardware antecipadamente | Criação de servidores sob demanda |
| Alto investimento inicial | Pagamento conforme o uso |
| Implantação pode levar semanas ou meses | Instâncias disponíveis em minutos |
| Capacidade limitada ao hardware adquirido | Escalabilidade conforme a demanda |
| Empresa é responsável por toda a infraestrutura | AWS gerencia a infraestrutura física |

No modelo **on-premises**, a empresa precisa adquirir servidores, aguardar a entrega, realizar a instalação e configurar toda a infraestrutura antes de começar a utilizá-la.

Com o **Amazon EC2**, basta provisionar uma instância e ela estará pronta para uso em poucos minutos.

---

# Benefícios do Amazon EC2

Os principais benefícios do EC2 são:

- **Elasticidade:** aumenta ou reduz a capacidade conforme a demanda.
- **Escalabilidade:** suporta desde pequenas aplicações até grandes ambientes com milhares de instâncias.
- **Agilidade:** servidores podem ser criados rapidamente.
- **Economia:** pagamento apenas pelo tempo de utilização.
- **Flexibilidade:** diferentes configurações de CPU, memória, armazenamento e rede para atender diferentes workloads.

---

# Como o Amazon EC2 funciona

O processo básico de utilização do EC2 pode ser dividido em três etapas.

## 1. Iniciar uma instância

O primeiro passo é criar uma instância (servidor virtual).

Para isso, é necessário definir:

- **AMI (Amazon Machine Image):** modelo da instância que contém o sistema operacional (Linux ou Windows) e, opcionalmente, softwares pré-instalados.
- **Tipo de instância:** define os recursos de hardware disponíveis, como CPU, memória e desempenho de rede.

---

## 2. Conectar-se à instância

Após a criação, é possível acessar o servidor para administrá-lo.

As principais formas de conexão são:

- **SSH:** para instâncias Linux.
- **RDP (Remote Desktop Protocol):** para instâncias Windows.
- **AWS Systems Manager:** serviço da AWS que permite acessar instâncias de forma mais segura e simplificada, sem a necessidade de acesso direto via SSH ou RDP.

## 3. Utilizar a instância

Depois de conectada, a instância pode ser utilizada como um servidor convencional.

É possível:

- Executar aplicações.
- Instalar programas.
- Criar arquivos e diretórios.
- Configurar serviços.
- Adicionar armazenamento.
- Executar comandos administrativos.

---

## Conceitos importantes

- **Instância:** servidor virtual executado no Amazon EC2.
- **AMI (Amazon Machine Image):** imagem utilizada como modelo para criar uma instância.
- **Tipo de instância:** configuração de hardware (CPU, memória e rede) da instância.
- **Provisionar:** criar e disponibilizar uma instância para uso.
- **Escalar:** aumentar ou reduzir os recursos utilizados conforme a necessidade.

---

## 4. Tipos de Instâncias do Amazon EC2

Ao criar uma instância do EC2, é necessário escolher um **tipo de instância**, que define a quantidade de CPU, memória, armazenamento e recursos de rede disponíveis.

Cada tipo é otimizado para diferentes cargas de trabalho.

| Tipo de instância | Características | Casos de uso |
|-------------------|-----------------|--------------|
| **Uso Geral (General Purpose)** | Equilíbrio entre CPU, memória e rede. | Servidores web, repositórios de código, aplicações de uso geral e cargas de trabalho variadas. |
| **Otimizada para Computação (Compute Optimized)** | Maior capacidade de processamento (CPU). | Servidores de jogos, computação de alto desempenho (HPC), simulações científicas e Machine Learning. |
| **Otimizada para Memória (Memory Optimized)** | Grande quantidade de memória RAM. | Bancos de dados de alto desempenho, Big Data e aplicações de análise de dados. |
| **Computação Acelerada (Accelerated Computing)** | Utiliza aceleradores de hardware, como GPUs. | Processamento gráfico, cálculos complexos, inteligência artificial e Machine Learning. |
| **Otimizada para Armazenamento (Storage Optimized)** | Alto desempenho para acesso a dados armazenados localmente. | Grandes bancos de dados, data warehouses e aplicações com alta taxa de leitura e gravação (I/O). |

> **Como escolher?**
>
> - Precisa de equilíbrio entre CPU e memória → **Uso Geral**.
> - Precisa de muito processamento → **Otimizada para Computação**.
> - Precisa de muita memória RAM → **Otimizada para Memória**.
> - Precisa de GPU → **Computação Acelerada**.
> - Precisa de acesso rápido ao armazenamento → **Otimizada para Armazenamento**.

---

## 5. Interagir com os Serviços da AWS

Todas as interações com os serviços da AWS são realizadas por meio de **APIs (Application Programming Interfaces)**.

A AWS oferece três principais formas de acessar e gerenciar seus serviços:

---

## Console de Gerenciamento da AWS

O **Console de Gerenciamento da AWS** é uma interface web que permite gerenciar os serviços da AWS por meio de uma interface visual.

Principais características:

- Acesso rápido aos serviços.
- Ferramenta de pesquisa de serviços.
- Fluxos de trabalho simplificados.
- Monitoramento de recursos.
- Visualização de alertas e faturamento.
- Disponível também em aplicativo móvel.

**Ideal para:**

Usuários que preferem uma interface gráfica para criar, configurar e acompanhar recursos da AWS.

---

## AWS CLI (Command Line Interface)

A **AWS CLI** permite gerenciar serviços da AWS diretamente pelo terminal.

Pode ser utilizada em:

- Windows.
- macOS.
- Linux.

Principais características:

- Execução de comandos diretamente no terminal.
- Automação de tarefas por scripts.
- Gerenciamento eficiente de vários recursos.

**Exemplo:**

Criar, iniciar ou parar instâncias do Amazon EC2 usando comandos.

**Ideal para:**

Desenvolvedores e usuários avançados que precisam automatizar processos e gerenciar recursos em grande escala.

---

## AWS SDK (Software Development Kit)

O **AWS SDK** permite integrar serviços da AWS diretamente dentro de aplicações.

Ele fornece bibliotecas e APIs para diversas linguagens de programação, como:

- Java.
- C++.
- .NET.
- Python.

Principais características:

- Integração de aplicações com serviços AWS.
- Automação de operações através de código.
- Documentação e exemplos para facilitar o desenvolvimento.

**Ideal para:**

Desenvolvedores que desejam utilizar serviços AWS dentro de suas próprias aplicações.

---

# Computação e o Modelo de Responsabilidade Compartilhada

O modelo de responsabilidade compartilhada define quais tarefas de segurança pertencem à AWS e quais pertencem ao cliente.

> **AWS é responsável pela segurança DA nuvem.**  
> **O cliente é responsável pela segurança NA nuvem.**

---

# Amazon EC2 e Responsabilidades

O Amazon EC2 é considerado um serviço com menor nível de gerenciamento pela AWS.

Isso significa que o cliente possui maior controle, mas também assume mais responsabilidades de configuração e segurança.

Ao utilizar uma instância EC2, o cliente é responsável por:

- Configurar a segurança da instância.
- Gerenciar o sistema operacional.
- Aplicar atualizações e patches.
- Configurar regras de firewall (Security Groups).
- Proteger aplicações e dados.

---

# Divisão de Responsabilidades no EC2

| Responsabilidade do Cliente | Responsabilidade da AWS |
|-----------------------------|-------------------------|
| Dados do cliente | Software da infraestrutura AWS |
| Criptografia dos dados do lado do cliente | Hardware |
| Criptografia no lado do servidor | Infraestrutura global da AWS |
| Proteção do tráfego de rede | Computação, armazenamento, banco de dados e redes |
| Gerenciamento de aplicações | |
| Configuração do sistema operacional | |
| Configuração da rede e firewall | |

---

# Amazon Machine Image (AMI)

Uma **Amazon Machine Image (AMI)** é um modelo pré-configurado utilizado para criar instâncias do Amazon EC2. Ela define a configuração inicial do servidor, permitindo criar múltiplas instâncias com as mesmas características.

## Componentes de uma AMI

Uma AMI pode incluir:

- Sistema operacional (Linux ou Windows).
- Configuração de armazenamento.
- Arquitetura da máquina.
- Permissões de inicialização.
- Aplicações e softwares pré-instalados.

Como todas as instâncias criadas a partir da mesma AMI utilizam a mesma configuração base, é possível garantir ambientes consistentes e padronizados.

---

## Formas de utilizar uma AMI

Existem três maneiras principais de utilizar uma AMI:

1. **Criar sua própria AMI:** ideal para ambientes personalizados, contendo configurações e softwares específicos da aplicação.
2. **Utilizar uma AMI fornecida pela AWS:** imagens oficiais com sistemas operacionais e softwares amplamente utilizados.
3. **Utilizar uma AMI do AWS Marketplace:** imagens disponibilizadas por parceiros da AWS, contendo softwares especializados e soluções prontas para uso.

---

## Vantagens das AMIs

O uso de AMIs proporciona:

- **Padronização:** todas as instâncias possuem a mesma configuração inicial.
- **Repetibilidade:** ambientes de desenvolvimento, testes e produção permanecem consistentes.
- **Escalabilidade:** novas instâncias podem ser criadas rapidamente.
- **Redução de erros:** evita configurações manuais repetitivas.
- **Facilidade de gerenciamento:** simplifica a administração de ambientes com muitas instâncias.

> **Resumo:** Pense na AMI como um **molde** de um servidor. Sempre que uma nova instância é criada a partir desse molde, ela nasce com a mesma configuração, garantindo consistência e facilitando a escalabilidade.

---

# Modalidades de Preços do Amazon EC2

A AWS oferece diferentes modelos de precificação para atender diferentes tipos de carga de trabalho. A escolha do modelo ideal depende da previsibilidade da demanda, da necessidade de disponibilidade e do orçamento.

| Modalidade | Quando utilizar | Principal benefício |
|------------|-----------------|---------------------|
| **Sob Demanda (On-Demand)** | Cargas de trabalho variáveis ou temporárias | Paga apenas pelo tempo de uso, sem compromisso de longo prazo. |
| **Instâncias Reservadas (Reserved Instances - RI)** | Cargas de trabalho estáveis e previsíveis | Economia de até **75%** com compromisso de 1 ou 3 anos. |
| **Instâncias Spot** | Workloads flexíveis e tolerantes a interrupções | Economia de até **90%**, utilizando capacidade ociosa da AWS. |
| **Savings Plans** | Uso consistente de computação | Economia de até **72%** com maior flexibilidade que as Instâncias Reservadas. |
| **Hosts Dedicados** | Aplicações com requisitos de conformidade ou licenciamento | Servidor físico exclusivo com controle total sobre o hardware. |
| **Instâncias Dedicadas** | Necessidade de isolamento físico | Instâncias executadas em hardware dedicado à sua conta, sem controle do servidor físico. |

---

# Hosts Dedicados x Instâncias Dedicadas

Embora os nomes sejam parecidos, existem diferenças importantes.

| Hosts Dedicados | Instâncias Dedicadas |
|-----------------|----------------------|
| Servidor físico exclusivo. | Hardware isolado para sua conta. |
| Controle sobre o servidor físico e a alocação das instâncias. | Não há controle sobre qual servidor físico será utilizado. |
| Indicado para requisitos de licenciamento e conformidade. | Indicado quando apenas o isolamento físico é necessário. |

> **Resumo:**  
> **Host Dedicado = servidor físico exclusivo com controle total.**  
> **Instância Dedicada = isolamento físico, mas a AWS gerencia o servidor.**

---

# Otimização de Custos

A AWS oferece opções para reduzir custos de acordo com o perfil da carga de trabalho.

## Savings Plans

Ideal para aplicações com uso consistente.

Características:

- Economia de até **72%**.
- Compromisso de uso por **1 ou 3 anos**.
- Flexível entre diferentes tipos de instâncias e serviços (EC2, AWS Lambda, AWS Fargate e Amazon SageMaker).
- Opções de pagamento antecipado, parcial ou sem entrada.

---

## Reservas de Capacidade do Amazon EC2

Ideal para aplicações críticas que precisam garantir capacidade disponível.

Características:

- Reserva capacidade em uma **Zona de Disponibilidade (AZ)** específica.
- Garante que haverá recursos disponíveis quando necessário.
- A capacidade reservada é cobrada mesmo que não esteja sendo utilizada.
- As instâncias executadas seguem o preço Sob Demanda.

---

## Instâncias Reservadas (Reserved Instances)

Ideal para cargas de trabalho estáveis e previsíveis.

Características:

- Economia de até **75%** em relação ao modelo Sob Demanda.
- Compromisso de **1 ou 3 anos**.
- O desconto pode ser aplicado automaticamente a diferentes tamanhos de instâncias da mesma família dentro da mesma Região.
- Também pode ser utilizado em diferentes Zonas de Disponibilidade da mesma Região.

---

## Resumo

- **Sob Demanda:** máxima flexibilidade, sem compromisso.
- **Reservada (RI):** melhor opção para uso contínuo e previsível.
- **Spot:** maior economia, mas a instância pode ser interrompida pela AWS.
- **Savings Plans:** economia com mais flexibilidade que as Instâncias Reservadas.
- **Host Dedicado:** servidor físico exclusivo.
- **Instância Dedicada:** isolamento físico sem controle do servidor.
- **Reserva de Capacidade:** garante disponibilidade de recursos para workloads críticos.

---

# Escalabilidade e Elasticidade

Embora os termos sejam parecidos, eles representam conceitos diferentes na computação em nuvem.

| Escalabilidade | Elasticidade |
|---------------|--------------|
| Aumenta a capacidade de um sistema para suportar crescimento ao longo do tempo. | Ajusta automaticamente os recursos conforme a demanda em tempo real. |
| Planejamento de longo prazo. | Resposta automática a variações momentâneas de carga. |
| Pode aumentar recursos vertical ou horizontalmente. | Adiciona ou remove recursos conforme necessário. |

---

## Escalabilidade

A **escalabilidade** é a capacidade de expandir a infraestrutura para suportar um aumento contínuo na carga de trabalho.

Existem duas formas de escalar:

- **Escala vertical (Scale Up):** aumenta os recursos de uma máquina existente, como CPU ou memória.
- **Escala horizontal (Scale Out):** adiciona novas instâncias à infraestrutura.

**Objetivo:** permitir que a aplicação cresça de forma planejada conforme aumenta o número de usuários ou o volume de processamento.

---

## Elasticidade

A **elasticidade** permite que a infraestrutura aumente ou reduza recursos automaticamente de acordo com a demanda.

Por exemplo:

- Em horários de pico, novas instâncias são criadas automaticamente.
- Quando a demanda diminui, as instâncias excedentes são removidas.

**Benefícios:**

- Melhor aproveitamento dos recursos.
- Redução de custos.
- Melhor desempenho da aplicação.

---

# Amazon EC2 Auto Scaling

O **Amazon EC2 Auto Scaling** ajusta automaticamente a quantidade de instâncias EC2 para acompanhar as mudanças na demanda da aplicação.

Ele ajuda a manter a aplicação disponível e evita desperdício de recursos.

Existem duas formas de escalonamento:

- **Escalonamento Dinâmico:** adiciona ou remove instâncias automaticamente conforme a demanda em tempo real.
- **Escalonamento Preditivo:** utiliza previsões de uso para provisionar instâncias antes que o aumento de demanda aconteça.

---

# Grupo de Auto Scaling

O Auto Scaling organiza as instâncias em um **Grupo de Auto Scaling (Auto Scaling Group)**, que controla quantas instâncias devem estar em execução.

Ao configurar um grupo, são definidos três valores principais:

| Configuração | Descrição |
|--------------|-----------|
| **Capacidade mínima** | Número mínimo de instâncias que permanecerão em execução. Também é a quantidade criada inicialmente, caso nenhuma capacidade desejada seja definida. |
| **Capacidade desejada** | Quantidade ideal de instâncias que o Auto Scaling tentará manter para atender à demanda atual. |
| **Capacidade máxima** | Limite máximo de instâncias que podem ser criadas, evitando custos excessivos. |

---

## Exemplo

Imagine uma aplicação configurada com:

- **Capacidade mínima:** 2 instâncias.
- **Capacidade desejada:** 4 instâncias.
- **Capacidade máxima:** 10 instâncias.

Em um período de alta demanda, o Auto Scaling poderá aumentar gradualmente o número de instâncias até o limite de **10**.

Quando o tráfego diminuir, as instâncias extras serão encerradas automaticamente, mas a aplicação nunca ficará com menos de **2** instâncias em execução.

---

# Benefícios do EC2 Auto Scaling

- Ajusta automaticamente a infraestrutura conforme a demanda.
- Mantém a alta disponibilidade da aplicação.
- Evita desperdício de recursos.
- Reduz custos operacionais.
- O cliente paga apenas pelas instâncias que permanecerem em execução.

> **Resumo:** A **escalabilidade** permite aumentar a capacidade de uma aplicação, enquanto a **elasticidade** permite ajustar essa capacidade automaticamente conforme a demanda. O **Amazon EC2 Auto Scaling** combina esses conceitos para manter o desempenho da aplicação com o menor custo possível.

---

# Elastic Load Balancing (ELB)

O **Elastic Load Balancing (ELB)** é um serviço da AWS que distribui automaticamente o tráfego de entrada entre várias instâncias do Amazon EC2.

Seu principal objetivo é melhorar o desempenho, a disponibilidade e a confiabilidade das aplicações, evitando que uma única instância fique sobrecarregada.

O ELB atua como um **ponto único de entrada** para a aplicação: todas as requisições passam primeiro pelo balanceador, que decide para qual instância elas serão enviadas.

> **Resumo:** O ELB distribui o tráfego entre várias instâncias EC2 para manter a aplicação disponível e com bom desempenho.

---

# ELB e Auto Scaling

Embora sejam serviços independentes, o **Elastic Load Balancing** e o **Amazon EC2 Auto Scaling** normalmente trabalham juntos.

- O **Auto Scaling** cria ou remove instâncias conforme a demanda.
- O **ELB** distribui automaticamente as requisições entre essas instâncias.

Essa combinação permite que a aplicação aumente ou reduza sua capacidade sem interromper o atendimento aos usuários.

---

# Benefícios do Elastic Load Balancing

- **Distribuição eficiente do tráfego:** evita que uma única instância receba todas as requisições.
- **Escalabilidade automática:** funciona em conjunto com o Auto Scaling, acompanhando a criação e remoção de instâncias.
- **Gerenciamento simplificado:** reduz a necessidade de configuração manual e auxilia em tarefas como manutenção e failover.

---

# Métodos de Roteamento

O ELB pode utilizar diferentes estratégias para distribuir as requisições.

| Método | Funcionamento |
|---------|---------------|
| **Round Robin** | Distribui as requisições de forma sequencial e uniforme entre todas as instâncias. |
| **Menor Número de Conexões** | Direciona o tráfego para a instância com menos conexões ativas. |
| **Hash de IP** | Utiliza o endereço IP do cliente para encaminhar as requisições sempre para a mesma instância. |
| **Menor Tempo de Resposta** | Envia a requisição para a instância que responde mais rapidamente. |

---

# Exemplo

Imagine um portal de um hospital para agendamento de consultas.

- **Baixa demanda:** poucas pessoas acessam o sistema e algumas instâncias EC2 são suficientes.
- **Alta demanda:** em horários de pico, o Auto Scaling cria novas instâncias automaticamente.
- O **Elastic Load Balancing** passa a distribuir as requisições entre todas as instâncias disponíveis, evitando sobrecarga em qualquer servidor.

Quando o tráfego diminui, o Auto Scaling remove as instâncias excedentes, enquanto o ELB continua distribuindo o tráfego entre as instâncias restantes.

---

# Resumo

- O **ELB** distribui automaticamente o tráfego entre várias instâncias.
- Atua como um ponto único de entrada para a aplicação.
- Trabalha em conjunto com o **Amazon EC2 Auto Scaling**.
- Melhora a disponibilidade, o desempenho e a escalabilidade da aplicação.
- Utiliza diferentes algoritmos para balancear as requisições de forma eficiente.

---

# Serviços de Desacoplamento

Em aplicações modernas, é importante que os componentes funcionem de forma independente. Isso aumenta a disponibilidade, a escalabilidade e a resiliência do sistema.

---

# Aplicação Monolítica x Microsserviços

| Aplicação Monolítica | Arquitetura de Microsserviços |
|----------------------|-------------------------------|
| Todos os componentes são fortemente acoplados. | Os componentes são independentes (baixo acoplamento). |
| A falha de um componente pode afetar toda a aplicação. | A falha de um componente não impede o funcionamento dos demais. |
| Mais difícil de escalar e manter. | Mais flexível, escalável e resiliente. |

> **Resumo:** Em uma arquitetura de microsserviços, cada componente pode funcionar de forma independente, reduzindo o impacto de falhas.

---

# Comunicação entre Microsserviços

A AWS oferece serviços que permitem a comunicação entre diferentes partes de uma aplicação de forma confiável e escalável.

Os principais são:

- **Amazon EventBridge**
- **Amazon SQS**
- **Amazon SNS**

Cada serviço atende a uma necessidade diferente.

---

# Amazon EventBridge

O **Amazon EventBridge** é um serviço de eventos que conecta diferentes aplicações e serviços.

Quando um evento acontece (por exemplo, um pedido realizado), o EventBridge identifica esse evento e o encaminha automaticamente para os serviços responsáveis.

### Principais benefícios

- Comunicação baseada em eventos.
- Integração entre serviços AWS, aplicações e parceiros.
- Filtragem e roteamento de eventos.
- Maior desacoplamento entre os componentes da aplicação.

**Exemplo:**

Em um aplicativo de entrega de comida, quando um cliente faz um pedido, o EventBridge envia esse evento para diferentes serviços, como:

- Processamento do pagamento.
- Restaurante.
- Controle de estoque.
- Sistema de entrega.

Cada serviço recebe apenas o evento que precisa processar e trabalha de forma independente.

---

# Amazon SQS (Simple Queue Service)

O **Amazon SQS** é um serviço de filas de mensagens.

Seu objetivo é armazenar mensagens até que outro sistema esteja disponível para processá-las.

### Funcionamento

1. Um produtor envia uma mensagem para uma fila.
2. A mensagem permanece armazenada.
3. Um consumidor recupera a mensagem quando estiver disponível.
4. Após o processamento, a mensagem é removida da fila.

### Benefícios

- Evita perda de mensagens.
- Permite comunicação assíncrona.
- Reduz gargalos entre sistemas.
- Aumenta a confiabilidade das aplicações.

**Exemplo:**

Uma equipe de suporte registra chamados em uma fila. Mesmo que o especialista esteja ocupado, novos chamados continuam sendo armazenados até que possam ser processados.

---

# Amazon SNS (Simple Notification Service)

O **Amazon SNS** é um serviço de notificações baseado no modelo **Publicação/Assinatura (Publish/Subscribe)**.

As mensagens são publicadas em um **tópico**, e todos os assinantes desse tópico recebem a notificação.

Os assinantes podem ser:

- E-mail.
- Aplicações.
- AWS Lambda.
- Servidores.
- Outros serviços AWS.

### Benefícios

- Envio de notificações para vários destinatários ao mesmo tempo.
- Comunicação rápida.
- Fácil integração com outros serviços.

**Exemplo:**

Uma empresa cria três tópicos:

- Novos produtos.
- Promoções.
- Eventos.

Cada cliente escolhe quais tópicos deseja assinar e recebe apenas as notificações de seu interesse.

---

# Comparação dos Serviços

| Serviço | Principal função | Exemplo |
|----------|------------------|----------|
| **Amazon EventBridge** | Rotear eventos entre aplicações e serviços. | Pedido realizado dispara pagamento, estoque e entrega. |
| **Amazon SQS** | Armazenar mensagens em filas para processamento posterior. | Fila de chamados de suporte. |
| **Amazon SNS** | Enviar notificações para vários assinantes simultaneamente. | Envio de promoções por e-mail para clientes inscritos. |

---

# Resumo

- **EventBridge:** conecta aplicações por meio de **eventos**.
- **SQS:** permite comunicação por **filas de mensagens**, garantindo processamento confiável.
- **SNS:** envia **notificações** para vários assinantes utilizando o modelo **Publish/Subscribe**.

Os três serviços ajudam a construir aplicações desacopladas, escaláveis e resilientes.