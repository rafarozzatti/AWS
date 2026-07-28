# AWS Cloud Practitioner Essentials - Módulo 4

## Alcance global com a infraestrutura da AWS (resumido)
- Escolha da Região: Selecione a Região AWS considerando fatores como latência, proximidade dos usuários, custos e requisitos legais/compliance.
- Locais da borda (Edge Locations): Armazenam conteúdo em cache (imagens, vídeos e outros arquivos) para reduzir a latência e acelerar a entrega aos usuários.
- AWS CloudFormation (IaC): Serviço de Infraestrutura como Código (Infrastructure as Code - IaC) que automatiza a criação e implantação de recursos, garantindo ambientes consistentes e padronizados.

---

## Principais considerações ao escolher uma Região AWS
- Conformidade: Escolha uma Região que atenda às leis e regulamentações de proteção de dados (ex.: LGPD, GDPR).
- Proximidade: Escolha Regiões próximas aos usuários para reduzir a latência.
- Disponibilidade de recursos: Verifique se os serviços e recursos necessários estão disponíveis na Região.
Preços: Os custos variam entre as Regiões, podendo impactar o valor da infraestrutura.

---

## Concepção de arquiteturas altamente disponíveis
Implantação Multi-Região e Multi-AZ: Distribuir recursos em múltiplas Regiões e Zonas de Disponibilidade (AZs) aumenta a alta disponibilidade, a redundância e a tolerância a falhas.

### Conceitos
- Alta disponibilidade: A aplicação continua funcionando mesmo se ocorrer falha em um componente ou AZ.
- Agilidade: Capacidade de implantar e modificar recursos rapidamente.
- Elasticidade: Capacidade de aumentar ou reduzir recursos automaticamente conforme a demanda.

### Locais da borda
São locais distribuídos globalmente que armazenam conteúdo em cache para reduzir a latência e acelerar a entrega de dados, utilizando serviços como o Amazon CloudFront (CDN).

### Elementos da infraestrutura global da AWS
- Regiões: Locais físicos da AWS, cada um com 3 ou mais Zonas de Disponibilidade.
- Zonas de Disponibilidade (AZs): Um ou mais data centers isolados, com energia, rede e conectividade independentes.
- Locais da borda (Edge Locations): Pontos de presença que armazenam conteúdo em cache para entrega mais rápida aos usuários.

---

## AWS CloudFormation

O AWS CloudFormation é um serviço de Infraestrutura como Código (IaC) que permite criar, configurar e gerenciar recursos da AWS por meio de templates, automatizando a implantação da infraestrutura.

### Formas de interagir com os serviços da AWS
- Console de Gerenciamento da AWS: Interface gráfica (GUI) para criar e gerenciar recursos.
- AWS CLI: Linha de comando para administrar e automatizar recursos com scripts.
- AWS SDK: Bibliotecas para integrar serviços da AWS em aplicações.
- AWS CloudFormation: Ferramenta de IaC para criar e gerenciar infraestrutura automaticamente e de forma padronizada.

### Casos de uso
- AWS CLI: Automatização de tarefas e scripts.
- AWS SDK: Integração de aplicações com os serviços da AWS.
- Console: Gerenciamento visual dos recursos.
- CloudFormation: Implantação automatizada, consistente e reproduzível da infraestrutura, muito usado em DevOps e CI/CD.
