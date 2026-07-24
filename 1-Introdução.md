# AWS Cloud Practitioner Essentials - Módulo 1

## 1. Introdução à AWS

A **Amazon Web Services (AWS)** é uma plataforma de computação em nuvem que fornece recursos de tecnologia da informação sob demanda pela internet.

A AWS oferece centenas de serviços para diferentes necessidades, como:

- Computação
- Armazenamento
- Bancos de dados
- Redes
- Inteligência Artificial (IA)
- Machine Learning
- Análise de dados
- Segurança
- Entrega de conteúdo

A AWS é uma das maiores plataformas de nuvem do mundo e é utilizada por empresas de todos os tamanhos, desde startups até grandes corporações e órgãos governamentais.

---

# 2. Modelo Cliente-Servidor

Antes de entender a nuvem, é importante compreender o modelo cliente-servidor.

Nesse modelo:

1. O cliente faz uma requisição.
2. O servidor recebe a requisição.
3. O servidor valida se ela pode ser atendida.
4. O servidor processa a solicitação.
5. O servidor retorna uma resposta ao cliente.

Exemplo:

Uma aplicação solicita informações de um banco de dados.

Fluxo:

```
Cliente → Solicitação → Servidor

Servidor → Resposta → Cliente
```

## Analogia da cafeteria

Imagine que um cliente entra na cafeteria e faz um pedido de café. A barista recebe esse pedido, verifica se ele é válido (por exemplo, se o cliente realizou o pagamento e se o item existe no cardápio), prepara a bebida e a entrega ao cliente.

Na analogia:

| Cafeteria | Computação |
|-----------|------------|
| Cliente fazendo pedido | Usuário/aplicação fazendo uma requisição |
| Pedido de café | Solicitação |
| Barista | Servidor |
| Preparação do café | Processamento da solicitação |
| Café entregue | Resposta |

O cliente solicita algo e o servidor responde, desde que a solicitação seja válida.

## Pague Apenas Pelo Que Usar

Outro conceito importante apresentado com a analogia da cafeteria é o modelo de cobrança da AWS.

Imagine que uma cafeteria contrata funcionários conforme a quantidade de clientes:

- Em dias movimentados, mais baristas são necessários.
- Em dias tranquilos, menos funcionários trabalham.

Assim, o proprietário paga apenas pelas horas realmente trabalhadas, evitando custos desnecessários com funcionários ociosos.

Na AWS acontece o mesmo com os recursos computacionais:

- Os recursos são **provisionados** quando há necessidade.
- Quando deixam de ser necessários, podem ser **desprovisionados** rapidamente.
- Após serem removidos, a cobrança é interrompida.

Esse modelo elimina a necessidade de comprar infraestrutura antecipadamente, como acontece em ambientes **on-premises**, onde os servidores precisam ser adquiridos antes mesmo de saber a demanda real.

### Conceitos importantes

- **Provisionar:** criar e disponibilizar um recurso (servidor, banco de dados, armazenamento etc.).
- **Desprovisionar:** remover um recurso que não está mais sendo utilizado.

> **Resumo:** Na AWS você paga apenas pelos recursos utilizados e somente pelo tempo em que eles permanecem ativos, permitindo escalar a infraestrutura conforme a demanda e reduzindo desperdícios.

---

# 3. O que é Computação em Nuvem?

A AWS ú uma plataforma de computação em nuvem que disponibiliza serviços pela internet, como servidores virtuais, armazenamento, banco de dados, redes, inteligência artificial, segurança e muitos outros recursos. O cliente paga apenas pelo que utiliza e pode aumetar ou reduzir os recursos de acordo com a demanda, sem pecisar comprar ou manter infraestrutura física.

---

# 4. Tipos de Implantação na Nuvem

Existem três principais modelos de implantação de recursos de TI:

### ☁️ Nuvem (Cloud)

Todos os recursos ficam na nuvem. Oferece escalabilidade, flexibilidade e pagamento conforme o uso.

### 🖥️ On-Premises

Os recursos ficam no datacenter da empresa. Oferece maior controle, mas menos benefícios da nuvem.

### 🔄 Híbrido

Combina recursos na nuvem e on-premises, permitindo integrar aplicações legadas com serviços em nuvem.

> **Resumo:**  
> - **Cloud:** tudo na nuvem.  
> - **On-Premises:** tudo na infraestrutura da empresa.  
> - **Híbrido:** combinação dos dois modelos.

---

# 5. Benefícios da AWS

A AWS possui seis principais benefícios.

---

## 5.1 Troca de despesas fixas por despesas variáveis

Paga apenas pelo que usa, sem grandes investimentos iniciais.

---

## 5.2 Economias massivas em escala

A infraestrutura da AWS reduz os custos para os clientes.

---

## 5.3 Escalabilidade

Aumenta ou reduz reursos conforme a demanda.

---

## 5.4 Agilidade

Impalnta aplicações e serviços rapidamente.

---

## 5.5 Sem manutenção de data centers

A AWS gerencia a infraestrutura física.

---

## 5.6 Alcance global

Implanta aplicações em várias regiões do mundo em poucos minutos.

---

# 6. Infraestrutura Global da AWS

A infraestrutura global da AWS consiste em locais físicos em todo o mundo que contêm grupos de data centers.

```
Região
 └── Zona de Disponibilidade (AZ)
      └── Datacenter
```

---

# 6.1 Região AWS

Locais físicos da AWS ao redor do mundo, cada uma com **no mínimo três Zonas de Disponibilidade (AZs)**.

Exemplos:

- São Paulo
- Tóquio
- Paris
- Ohio

Escolher uma região próxima aos usuários ajuda a reduzir a latência e melhorar o desempenho das aplicações.

---

# 6.2 Zona de Disponibilidade (AZ)

Um ou mais data centers isolados, com energia, rede e conctividade redundantes, garantindo alta disponibilidade, baixa latência e tolerância a flhas.

As AZs são separadas fisicamente para evitar que uma falha afete todas.

---

# 6.3 Alta Disponibilidade

A AWS oferece alta disponibilidade ao distrubuir recursos entre múltiplas Zonas de Disponibilidade (AZs). Como cada AZ é isolada e possui energia, rede e conectividade independentes, é recomendado distribuir os recursos entre elas. Assim, se uma AZ falhar, as aplicações continuam funcionando nas demais, garantindo redundância e tolerância a falhas.

---

# 7. Modelo de Responsabilidade Compartilhada

A segurança na AWS é dividida entre a AWS e o cliente, seguindo o **Modelo de Responsabilidade Compartilhada**.

> **AWS é responsável pela segurança DA nuvem.**  
> **O cliente é responsável pela segurança NA nuvem.**

Isso significa que a AWS protege toda a infraestrutura física que executa os serviços em nuvem, enquanto o cliente é responsável por proteger os recursos, dados e configurações que utiliza dentro da AWS.

## AWS: Segurança DA nuvem

A AWS é responsável por proteger a infraestrutura que executa os serviços da plataforma, incluindo:

- Datacenters.
- Hardware.
- Rede física.
- Infraestrutura.
- Serviços básicos da plataforma.

---

## Cliente: Segurança NA nuvem

O cliente é responsável por proteger e configurar corretamente os recursos que utiliza, incluindo:

- Dados.
- Usuários.
- Permissões.
- Aplicações.
- Configurações.
- Sistema operacional (quando aplicável).
- Criptografia (quando for responsabilidade do cliente).

> **Dica para memorizar:**  
> **A AWS protege a infraestrutura; o cliente protege tudo o que coloca e configura dentro dela.**
