<h1 align="center">📡 Tecnologias de Redes Locais - Avaliação 🖧</h1>

<p align="center">
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License">
  </a>
</p>

<p>
  Este projeto é uma avaliação prática da disciplina de <strong>Tecnologias de Redes Locais</strong> no curso de Tecnologia em Telemática, ministrada pelo professor <strong>Marcelo Portela Sousa</strong>. O objetivo é implementar uma topologia de rede que envolve configurações avançadas de agregação de enlaces, VLANs, endereçamento IPv4 e IPv6, RSTP, DHCP e o roteamento inter-VLAN por meio da técnica Router-on-a-Stick, utilizando um simulador de redes.
</p>

<h2>🔍 Requisitos e Funcionalidades 🎛️</h2>

### Agregação de Enlaces e LACP 🔗
Cinco agregações de enlaces com LACP ativo foram configuradas, cada uma com capacidade de 200 Mbps. Essas conexões são utilizadas para aumentar a largura de banda e fornecer redundância entre os switches.

As portas de agregação foram configuradas conforme o seguinte padrão:
- **po1**: SW1 (f0/11 e f0/12) <–> SW2 (f0/11 e f0/12)
- **po3**: SW1 (f0/10 e f0/13) <–> SW3 (f0/10 e f0/13)
- **po4**: SW1 (f0/8 e f0/14) <–> SW4 (f0/8 e f0/14)
- **po5**: SW2 (f0/3 e f0/23) <–> SW3 (f0/3 e f0/23)
- **po6**: SW2 (f0/10 e f0/24) <–> SW4 (f0/10 e f0/24)

### Configuração de VLANs e Sub-redes 🌐
Seis VLANs foram criadas e associadas a sub-redes, com faixas específicas para suportar diferentes quantidades de hosts:
- **VLAN 10**: 300 hosts
- **VLAN 20**: 260 hosts
- **VLAN 30**: 200 hosts
- **VLAN 40**: 50 hosts
- **VLAN 99**: 20 hosts
- **VLAN 199**: 20 hosts

### Modo de Operação das Portas 🔌
As portas de acesso e tronco foram configuradas para otimizar o tráfego entre switches:
- **Modo Acesso**: Usado para conectar PCs em VLANs específicas (VLAN 10, VLAN 20, VLAN 30, VLAN 40).
- **Modo Trunk**: Configurado para permitir a passagem de múltiplas VLANs em links de agregação.

### RSTP e Segurança 🔄
- RSTP foi habilitado para reduzir os tempos de convergência em caso de falhas na topologia.
- Portfast e BPDU Guard foram ativados nas interfaces conectadas aos PCs e ao roteador para evitar loops.

### Router-on-a-Stick e DHCP 📶
- Router-on-a-Stick configurado no R1, criando sub-interfaces para rotear o tráfego entre VLANs.
- Pools DHCP foram criados no roteador para atribuir endereços IP automaticamente aos dispositivos nas VLANs.

### Endereçamento IPv4 e IPv6 🧭
- Endereçamento IPv4 estático nas sub-interfaces de R1 e dinâmico via DHCP para os PCs.
- Endereçamento IPv6 estático nas sub-interfaces do R1, com demais dispositivos utilizando SLAAC para IPv6.

<h2>⚙️ Tecnologias Utilizadas 🛠️</h2>

-  Simulador de Redes (Packet Tracer)

<h2>🤝 Contribuição 🤝</h2>

Contribuições são bem-vindas! Se você tiver sugestões, correções de bugs ou novas funcionalidades, fique à vontade para abrir uma issue ou enviar um pull request.

<h2>📜 Licença 📜</h2>

<p>Este projeto está licenciado sob a MIT License.</p>

<h2>📘 Orientação 📘</h2>

<p>Este projeto foi desenvolvido sob a orientação do professor Marcelo Portela Sousa para a disciplina de Tecnologias de Redes Locais.</p>

<h2>✉️ Contato ✉️</h2>
Se você tiver alguma dúvida ou quiser saber mais sobre o projeto, sinta-se à vontade para entrar em contato através do meu perfil no GitHub ou mande uma mensagem para o seguinte e-mail: <strong>joseffermax1472@gmail.com</strong>.

<h2 align="center">🌐 Explore a Topologia de Redes e Aprofunde-se nas Configurações! 🚀</h2>

