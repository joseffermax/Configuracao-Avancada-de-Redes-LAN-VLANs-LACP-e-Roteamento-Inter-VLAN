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

<h2>🔧 Pré-requisitos e Download do Simulador de Redes 🌐</h2>

Se você ainda não possui um simulador de redes para realizar testes com este cenário, recomendamos que baixe o **Cisco Packet Tracer**.

### Como Baixar o Cisco Packet Tracer
1. Acesse o site oficial da [Cisco Networking Academy](https://www.netacad.com/).
2. Crie uma conta gratuita, ou faça login caso já tenha uma.
3. Procure o **Cisco Packet Tracer** na seção de recursos e faça o download.

> **Nota**: O Packet Tracer é gratuito para uso acadêmico e é uma ótima ferramenta para praticar configurações de redes e protocolos.

### Cenário e Documentação 📄
O cenário de topologia de rede, junto com um PDF detalhado com instruções de configuração, está disponível para download:

- [Baixar Cenário Packet Tracer (.pkt)](https://github.com/joseffermax/Configura-o-Avancada-de-Redes-LAN-VLANs-LACP-e-Roteamento-Inter-VLAN/blob/main/Avalia%C3%A7%C3%A3o%20Tecnologias%20de%20Redes%20Locais.pkt)
- [Baixar PDF de Instruções (.pdf)](https://github.com/joseffermax/Configura-o-Avancada-de-Redes-LAN-VLANs-LACP-e-Roteamento-Inter-VLAN/blob/main/Avalia%C3%A7%C3%A3o%20Tecnologias%20de%20Redes%20Locais.pdf)

> ⚠️ **Importante**: Certifique-se de abrir o cenário no simulador de sua escolha para seguir as instruções e testar as configurações do projeto. Isso permitirá uma experiência prática e reforçará o entendimento dos conceitos aplicados.

<h2>⚙️ Tecnologias Utilizadas 🛠️</h2>

- Simulador de Redes (Packet Tracer)

<h2>🤝 Contribuição 🤝</h2>

Contribuições são bem-vindas! Se você tiver sugestões, correções de bugs ou novas funcionalidades, fique à vontade para abrir uma issue ou enviar um pull request.

<h2>📜 Licença 📜</h2>

<p>Este projeto está licenciado sob a MIT License.</p>

<h2>📘 Orientação 📘</h2>

<p>Este projeto foi desenvolvido sob a orientação do professor Marcelo Portela Sousa para a disciplina de Tecnologias de Redes Locais.</p>

<h2>✉️ Contato ✉️</h2>
Se você tiver alguma dúvida ou quiser saber mais sobre o projeto, sinta-se à vontade para entrar em contato através do meu perfil no GitHub ou mande uma mensagem para o seguinte e-mail: <strong>joseffermax1472@gmail.com</strong>.

<h2 align="center">🌐 Explore a Topologia de Redes e Aprofunde-se nas Configurações! 🚀</h2>

