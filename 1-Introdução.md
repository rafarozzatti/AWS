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

- O **cliente** faz uma solicitação.
- O **servidor** processa essa solicitação.
- O servidor retorna uma resposta ao cliente.

Exemplo:

Uma aplicação solicita informações de um banco de dados.

Fluxo:

```
Cliente → Solicitação → Servidor

Servidor → Resposta → Cliente
```

## Analogia da cafeteria

A cafeteria representa o modelo cliente-servidor:

| Cafeteria | Computação |
|-----------|------------|
| Cliente fazendo pedido | Usuário/aplicação fazendo uma requisição |
| Pedido de café | Solicitação |
| Barista | Servidor |
| Café entregue | Resposta |

O cliente solicita algo e o servidor responde, desde que a solicitação seja válida.

---

# 3. História da AWS

## Origem

No início dos anos 2000, a Amazon era uma empresa de comércio eletrônico.

Com o crescimento da plataforma, a equipe de tecnologia precisou aumentar constantemente:

- Servidores
- Armazenamento
- Capacidade computacional

Para resolver esses desafios, a Amazon criou ferramentas internas para tornar sua infraestrutura mais:

- Padronizada
- Eficiente
- Escalável

Em 2003, a empresa percebeu que outras organizações enfrentavam problemas semelhantes.

Assim surgiu a ideia de oferecer infraestrutura como serviço.

---

## Primeiros serviços AWS

| Ano | Serviço | Função |
|---|---|---|
| 2004 | Amazon SQS | Serviço de filas de mensagens |
| 2006 | Amazon S3 | Armazenamento de objetos |
| 2006 | Amazon EC2 | Computação escalável |

Inicialmente utilizada por startups e desenvolvedores, a AWS rapidamente cresceu e passou a atender:

- Empresas pequenas
- Grandes corporações
- Governos
- Organizações globais

---

# 4. O que é Computação em Nuvem?

A computação em nuvem é:

> A entrega sob demanda de recursos de TI pela internet, com pagamento conforme o uso.

Essa definição possui quatro conceitos principais:

---

## 4.1 Entrega sob demanda

Os recursos podem ser disponibilizados rapidamente conforme a necessidade.

Exemplo:

Uma empresa precisa de mais armazenamento.

Na AWS ela pode:

1. Criar o recurso.
2. Utilizar.
3. Remover quando não precisar mais.

Não é necessário comprar equipamentos antecipadamente.

---

## 4.2 Recursos de TI

Recursos de TI incluem:

- Servidores
- Armazenamento
- Bancos de dados
- Redes
- IA
- Machine Learning
- Aplicações

Esses recursos podem ser utilizados para criar e executar soluções.

---

## 4.3 Pela internet

Os recursos da AWS são acessados remotamente.

O usuário pode gerenciar sua infraestrutura:

- De casa
- Do trabalho
- De qualquer lugar do mundo

Basta possuir:

- Conexão com internet
- Conta AWS

---

## 4.4 Pagamento conforme utilização

Na AWS você paga somente pelos recursos utilizados.

Exemplo:

- Criou um servidor por algumas horas → paga por esse período.
- Removeu o servidor → deixa de pagar pelo uso.

Esse modelo evita grandes investimentos iniciais.

---

# 5. Datacenters

As aplicações precisam existir em uma infraestrutura física.

Essa infraestrutura fica localizada em **datacenters**.

Um datacenter é uma instalação física contendo:

- Servidores
- Equipamentos de rede
- Sistemas de armazenamento

Eles possuem:

- Energia redundante
- Refrigeração
- Segurança física
- Conectividade

Com a AWS, o cliente utiliza esses datacenters sem precisar construí-los ou gerenciá-los.

---

# 6. Modelos de Implantação

Existem três principais modelos de implantação:

---

# 6.1 Nuvem (Cloud)

Os recursos são hospedados na AWS.

Pode envolver:

- Migração de aplicações existentes.
- Criação de novas aplicações.

Exemplo:

Uma aplicação utilizando:

- Servidores virtuais
- Banco de dados
- Rede

Todos hospedados na AWS.

---

# 6.2 On-Premises

A empresa mantém sua própria infraestrutura física.

Características:

- Compra de hardware.
- Manutenção própria.
- Necessidade de espaço físico.
- Maior responsabilidade operacional.

Pode ser utilizado quando existem requisitos específicos, como baixa latência.

---

# 6.3 Híbrido

Combinação entre nuvem e infraestrutura própria.

Exemplo:

- Aplicação antiga continua no datacenter da empresa.
- Novos serviços utilizam a AWS.

É comum quando existem sistemas legados ou requisitos regulatórios.

---

# 7. Benefícios da AWS

A AWS possui seis principais benefícios.

---

## 7.1 Troca de despesas fixas por despesas variáveis

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

## 7.2 Economias massivas em escala

A AWS possui uma infraestrutura enorme e compra hardware em grande quantidade.

Isso permite:

- Melhores preços.
- Redução de custos.
- Disponibilização de tecnologia avançada para empresas de todos os tamanhos.

---

## 7.3 Parar de adivinhar capacidade

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

## 7.4 Velocidade e agilidade

A AWS permite criar ambientes rapidamente.

Benefícios:

- Testar novas ideias.
- Criar ambientes temporários.
- Inovar mais rápido.

Caso um teste não funcione:

- O recurso pode ser removido.
- O pagamento é interrompido.

---

## 7.5 Não manter datacenters

A AWS cuida da infraestrutura física.

A empresa não precisa gerenciar:

- Servidores físicos.
- Energia.
- Refrigeração.
- Equipamentos.

Assim, pode focar no próprio negócio.

---

## 7.6 Alcance global

A AWS possui infraestrutura espalhada pelo mundo.

Uma empresa pode disponibilizar aplicações em diferentes países sem construir novos datacenters.

Benefícios:

- Expansão internacional.
- Menor latência.
- Implantação rápida.

---

# 8. Infraestrutura Global da AWS

A infraestrutura AWS é organizada em:

```
Região
 └── Zona de Disponibilidade (AZ)
      └── Datacenter
```

---

# 8.1 Região AWS

Uma Região é uma localização geográfica onde a AWS possui infraestrutura.

Exemplos:

- São Paulo
- Tóquio
- Paris
- Ohio

Escolher uma região próxima aos usuários ajuda a reduzir latência.

---

# 8.2 Zona de Disponibilidade (AZ)

Uma AZ é formada por um ou mais datacenters.

Cada AZ possui:

- Energia independente.
- Rede independente.
- Conectividade redundante.

As AZs são separadas fisicamente para evitar que uma falha afete todas.

---

# 8.3 Alta Disponibilidade

Alta disponibilidade significa manter aplicações acessíveis com o mínimo de interrupção.

Para isso, utiliza-se:

- Redundância.
- Múltiplas AZs.
- Componentes alternativos.

---

# 8.4 Tolerância a Falhas

É a capacidade de continuar funcionando mesmo quando vários componentes apresentam falhas.

O objetivo é eliminar pontos únicos de falha.

---

# 8.5 Failover

Failover é transferir a operação para outro ambiente quando ocorre uma falha.

Exemplo:

Região São Paulo indisponível:

→ Aplicação passa para outra região.

---

# 9. Modelo de Responsabilidade Compartilhada

A segurança na AWS é dividida entre AWS e cliente.

## AWS: Segurança DA nuvem

A AWS é responsável por:

- Datacenters.
- Hardware.
- Rede física.
- Infraestrutura.
- Serviços básicos da plataforma.

---

## Cliente: Segurança NA nuvem

O cliente é responsável por:

- Dados.
- Usuários.
- Permissões.
- Aplicações.
- Configurações.
- Sistema operacional (quando aplicável).
- Criptografia quando for responsabilidade do cliente.

---

# 10. Exemplo Real: Empresa de E-commerce

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
