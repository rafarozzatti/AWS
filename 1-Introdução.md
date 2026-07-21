# AWS Cloud Practitioner Essentials - Introdução

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

## Pague Apenas Pelo Que Usar (Pay as You Go)

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

A computação em nuvem é:

> A entrega sob demanda de recursos de TI pela internet, com pagamento conforme o uso.

---

## Como funciona a computação em nuvem

Imagine que uma empresa precise de um servidor para hospedar uma aplicação.

Com a AWS, ela pode criar esse servidor em poucos minutos (**sob demanda**), acessá-lo e gerenciá-lo de qualquer lugar com uma conexão à internet (**pela internet**). Esse servidor é um dos diversos **recursos de TI** disponíveis na plataforma, assim como bancos de dados, armazenamento e redes. Quando o servidor não for mais necessário, basta removê-lo e a empresa deixa de pagar por ele (**pagamento conforme o uso**).

Esse modelo elimina a necessidade de comprar e manter infraestrutura física, tornando o uso dos recursos mais flexível e econômico.

---

# 4. Tipos de Implantação na Nuvem

Existem três principais modelos de implantação de recursos de TI:

### ☁️ Nuvem (Cloud)

Toda a infraestrutura é hospedada na nuvem. A empresa pode migrar aplicações existentes, criar novas aplicações ou combinar ambas as abordagens.

**Exemplo:** uma aplicação utiliza servidores, banco de dados e rede hospedados inteiramente na AWS.

### 🖥️ On-Premises

A infraestrutura é mantida no próprio datacenter da empresa. Esse modelo oferece maior controle sobre os recursos, mas exige que a organização seja responsável pela aquisição, manutenção e gerenciamento do hardware.

É utilizado quando há necessidade de recursos dedicados, baixa latência ou requisitos específicos de negócio.

### 🔄 Híbrido

Combina recursos on-premises e em nuvem. É indicado quando parte das aplicações precisa permanecer na infraestrutura local, enquanto outras utilizam os serviços da nuvem.

**Exemplo:** uma empresa mantém um sistema legado em seu datacenter, mas utiliza a AWS para processamento e análise de dados.

> **Resumo:**  
> - **Cloud:** tudo na nuvem.  
> - **On-Premises:** tudo na infraestrutura da empresa.  
> - **Híbrido:** combinação dos dois modelos.

---

# 5. Benefícios da AWS

A AWS possui seis principais benefícios.

---

## 5.1 Troca de despesas fixas por despesas variáveis

Modelo tradicional:

A empresa precisa investir antecipadamente em:

- Servidores
- Datacenter
- Equipamentos
- Manutenção

Mesmo que os recursos não sejam utilizados, o custo continua existindo.

Na AWS:

- O custo acompanha o uso.
- Não existe necessidade de grande investimento inicial.

Conceitos:

**CapEx:** investimento inicial em infraestrutura.

**OpEx:** despesas operacionais conforme utilização.

---

## 5.2 Economias massivas em escala

A AWS possui uma infraestrutura enorme e compra hardware em grande quantidade.

Isso permite:

- Melhores preços.
- Redução de custos.
- Disponibilização de tecnologia avançada para empresas de todos os tamanhos.

---

## 5.3 Parar de adivinhar capacidade

No modelo tradicional, empresas precisam prever crescimento.

Problemas:

### Excesso de capacidade

Compra de infraestrutura demais.

Resultado:

- Recursos ociosos.
- Dinheiro desperdiçado.

### Falta de capacidade

Infraestrutura insuficiente.

Resultado:

- Lentidão.
- Má experiência do usuário.

Na AWS:

- Recursos podem aumentar ou diminuir conforme a demanda.

---

## 5.4 Velocidade e agilidade

A AWS permite criar ambientes rapidamente.

Benefícios:

- Testar novas ideias.
- Criar ambientes temporários.
- Inovar mais rápido.

Caso um teste não funcione:

- O recurso pode ser removido.
- O pagamento é interrompido.

---

## 5.5 Não manter datacenters

A AWS cuida da infraestrutura física.

A empresa não precisa gerenciar:

- Servidores físicos.
- Energia.
- Refrigeração.
- Equipamentos.

Assim, pode focar no próprio negócio.

---

## 5.6 Alcance global

A AWS possui infraestrutura espalhada pelo mundo.

Uma empresa pode disponibilizar aplicações em diferentes países sem construir novos datacenters.

Benefícios:

- Expansão internacional.
- Menor latência.
- Implantação rápida.

---

# 6. Infraestrutura Global da AWS

A infraestrutura AWS é organizada em:

```
Região
 └── Zona de Disponibilidade (AZ)
      └── Datacenter
```

---

# 6.1 Região AWS

Uma Região é uma localização geográfica onde a AWS possui infraestrutura.

Exemplos:

- São Paulo
- Tóquio
- Paris
- Ohio

Escolher uma região próxima aos usuários ajuda a reduzir latência.

---

# 6.2 Zona de Disponibilidade (AZ)

Uma AZ é formada por um ou mais datacenters.

Cada AZ possui:

- Energia independente.
- Rede independente.
- Conectividade redundante.

As AZs são separadas fisicamente para evitar que uma falha afete todas.

---

# 6.3 Alta Disponibilidade

Alta disponibilidade significa manter aplicações acessíveis com o mínimo de interrupção.

Para isso, utiliza-se:

- Redundância.
- Múltiplas AZs.
- Componentes alternativos.

---

# 6.4 Tolerância a Falhas

É a capacidade de continuar funcionando mesmo quando vários componentes apresentam falhas.

O objetivo é eliminar pontos únicos de falha.

---

# 6.5 Failover

Failover é transferir a operação para outro ambiente quando ocorre uma falha.

Exemplo:

Região São Paulo indisponível:

→ Aplicação passa para outra região.

---

# 7. Modelo de Responsabilidade Compartilhada

A segurança na AWS é dividida entre a AWS e o cliente, seguindo o **Modelo de Responsabilidade Compartilhada**.

> **AWS é responsável pela segurança DA nuvem (Security OF the Cloud).**  
> **O cliente é responsável pela segurança NA nuvem (Security IN the Cloud).**

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

---

# 8. Exemplo Real: Empresa de E-commerce

Uma empresa deseja expandir globalmente.

Problema:

Quanto maior a distância entre o usuário e o servidor, maior a latência.

Solução:

Utilizar diferentes regiões AWS próximas dos clientes.

Exemplo:

- América do Sul → São Paulo
- Ásia → Singapura

---

## Alta disponibilidade no cenário

A empresa distribui sua aplicação em múltiplas AZs.

Se uma AZ falhar:

- Outra AZ continua funcionando.

---

## Segurança no cenário

A AWS protege:

- Datacenter.
- Hardware.
- Infraestrutura.

A empresa protege:

- Dados.
- Acesso.
- Criptografia.
- Configurações.

---

# Resumo Final

## Computação em nuvem

Entrega de recursos de TI pela internet, sob demanda e pagando pelo uso.

## AWS

Plataforma de nuvem que fornece infraestrutura global escalável.

## Principais benefícios

- Pague apenas pelo uso.
- Reduza custos.
- Escale conforme demanda.
- Inove rapidamente.
- Não gerencie datacenters.
- Alcance clientes globalmente.

## Infraestrutura

```
Região
 ↓
Zona de Disponibilidade
 ↓
Datacenter
```

## Segurança

```
AWS:
Segurança DA nuvem

Cliente:
Segurança NA nuvem
```
