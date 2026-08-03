## Componentes de rede

### Amazon VPC (Virtual Private Cloud)
A Amazon VPC é uma rede virtual privada e isolada na AWS, onde você define a configuração da rede para executar seus recursos com segurança.

### Sub-redes
As sub-redes dividem a VPC em partes menores e podem ser:
    - Sub-rede pública: Contém recursos acessíveis pela Internet, como servidores web.
    - Sub-rede privada: Contém recursos sem acesso direto à Internet, como bancos de dados.

---

## Organização de recursos na nuvem AWS

### Amazon VPC (Virtual Private Cloud)
A Amazon VPC é uma rede virtual privada e isolada, onde você cria e organiza seus recursos com segurança.

### Benefícios:
- Maior segurança.
- Controle de acesso aos recursos.
- Menor esforço para configurar e gerenciar a rede.

### Sub-redes
As sub-redes dividem a VPC em partes menores para organizar os recursos.
- Pública: Recursos acessíveis pela Internet.
- Privada: Recursos sem acesso direto à Internet.

### Gateway de Internet
Conecta a VPC à Internet, permitindo que recursos em sub-redes públicas sejam acessados externamente.

### Gateway Privado Virtual
Permite conectar uma VPC a uma rede privada (como um datacenter on-premises) por meio de uma VPN, garantindo comunicação segura e criptografada.

### VPN
Cria uma conexão criptografada entre uma rede privada e a VPC, protegendo os dados durante o tráfego pela Internet.
