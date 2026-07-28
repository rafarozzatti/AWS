# AWS Cloud Practitioner Essentials - Módulo 3

## Serviços gerenciados e não gerenciados

A AWS oferece diferentes níveis de gerenciamento, variando a responsabilidade entre a AWS e o cliente.

### Serviço não gerenciado:
- Cliente: Gerencia o sistema operacional, rede, firewall, aplicações, criptografia e dados.
- AWS: Gerencia a infraestrutura física (hardware, data centers e serviços da nuvem).

### Serviço gerenciado:
- Cliente: Gerencia os dados, acessos e parte da segurança.
- AWS: Gerencia a plataforma, sistema operacional, rede, firewall e infraestrutura.

### Serviço totalmente gerenciado:
- Cliente: Gerencia apenas o código, os dados e a criptografia do lado do cliente.
- AWS: Gerencia toda a infraestrutura, sistema operacional, escalabilidade, disponibilidade e segurança da plataforma.

---

## AWS Lambda (resumido)

O AWS Lambda é um serviço de computação sem servidor (serverless) que executa código em resposta a eventos, sem necessidade de provisionar ou gerenciar servidores. A AWS gerencia automaticamente a infraestrutura, o escalonamento e a disponibilidade, e você paga apenas pelo tempo de execução da função.

### Como funciona
1. Faça o upload do código como uma função Lambda.
2. Configure um evento para acionar a função (ex.: upload no S3, requisição HTTP, SNS).
3. O Lambda executa o código automaticamente quando o evento ocorre.
4. Você paga apenas pelo tempo de execução (em milissegundos).

### Casos de uso:
- Processamento de imagens.
- APIs e aplicações web.
- Processamento de eventos em tempo real.
- Automação de tarefas.
- Processamento de dados.

---

## Contêineres (resumido)

Os contêineres empacotam a aplicação e suas dependências em uma unidade portátil, garantindo consistência, portabilidade e escalabilidade.

### Contêineres × Máquinas Virtuais (VMs)
- Contêineres: Compartilham o sistema operacional do host, sendo mais leves e rápidos.
- VMs: Executam um sistema operacional completo, consumindo mais recursos.
Benefícios dos contêineres
- Consistência entre desenvolvimento, testes e produção.
- Implantações mais simples e confiáveis.
- Facilidade de escalabilidade.

### Orquestração

Ferramentas de orquestração automatizam a implantação, o gerenciamento e o escalonamento dos contêineres.

---

## Serviços de contêiner da AWS

- Amazon ECS (Elastic Container Service): Serviço de orquestração de contêineres da AWS.
    - ECS + EC2: Maior controle sobre a infraestrutura.
    - ECS + Fargate: Sem gerenciamento de servidores (serverless).
- Amazon EKS (Elastic Kubernetes Service): Serviço gerenciado de Kubernetes.
    - EKS + EC2: Controle total da infraestrutura.
    - EKS + Fargate: Kubernetes sem gerenciar servidores.
- Amazon ECR (Elastic Container Registry): Repositório para armazenar e gerenciar imagens de contêineres.
- AWS Fargate: Serviço de computação serverless para contêineres, utilizado com ECS e EKS, sem necessidade de gerenciar servidores.

---

## Outros serviços computacionais
- AWS Elastic Beanstalk: Serviço totalmente gerenciado para implantar, gerenciar e escalar aplicações web. A AWS cuida da infraestrutura, balanceamento de carga e monitoramento.
- AWS Batch: Serviço para executar e gerenciar workloads em lote (batch), escalando automaticamente os recursos conforme a necessidade.
- Amazon Lightsail: Serviço que oferece VPS, armazenamento, banco de dados e rede com preço mensal previsível. Ideal para pequenas aplicações e iniciantes.
- AWS Outposts: Solução de nuvem híbrida que leva a infraestrutura e os serviços da AWS para o datacenter local (on-premises).
