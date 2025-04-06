<h1 align="center">📡 Tecnologias de Redes Locais - Avaliação Prática 🖧</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Concluído-brightgreen.svg" alt="Status do Projeto">
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="Licença MIT">
  </a>
</p>

<p align="center">
  Projeto prático desenvolvido para a disciplina de <strong>Tecnologias de Redes Locais</strong> do curso de <strong>Tecnologia em Telemática</strong>, ministrada pelo professor <strong>Marcelo Portela Sousa</strong>.  
</p>

<p align="center">
  <strong>🔧 Topologia avançada com agregação de enlaces, VLANs, roteamento inter-VLAN, IPv4, IPv6 e muito mais!</strong>
</p>

---

## 🧠 Objetivo do Projeto

Este projeto tem como objetivo implementar e testar uma **topologia de rede LAN corporativa** utilizando recursos avançados de configuração em um ambiente simulado. Foram aplicados conceitos como:

- LACP (Link Aggregation Control Protocol)
- VLANs e Sub-redes
- RSTP
- DHCP
- Endereçamento IPv4 e IPv6
- Router-on-a-Stick
- Segurança em portas de acesso

O cenário foi implementado no **Cisco Packet Tracer**, simulador de redes amplamente utilizado em ambientes educacionais.

---

## 🚀 Funcionalidades Implementadas

### 🔗 Agregação de Enlaces com LACP

Configuração de 5 grupos de agregação (EtherChannel) com LACP ativo, cada um com 200 Mbps de banda, promovendo redundância e desempenho:

| EtherChannel | SW1 Portas | SW2/SW3/SW4 Portas |
|--------------|------------|--------------------|
| **po1**      | f0/11, f0/12 | SW2: f0/11, f0/12 |
| **po3**      | f0/10, f0/13 | SW3: f0/10, f0/13 |
| **po4**      | f0/8, f0/14  | SW4: f0/8, f0/14  |
| **po5**      | SW2: f0/3, f0/23 | SW3: f0/3, f0/23 |
| **po6**      | SW2: f0/10, f0/24 | SW4: f0/10, f0/24 |

---

### 🌐 VLANs e Sub-redes

Foram configuradas 6 VLANs com diferentes faixas de sub-redes, otimizando o tráfego e segmentando a rede conforme necessidade de hosts:

| VLAN | Quantidade de Hosts |
|------|----------------------|
| VLAN 10 | 300 |
| VLAN 20 | 260 |
| VLAN 30 | 200 |
| VLAN 40 | 50  |
| VLAN 99 | 20  |
| VLAN 199 | 20 |

---

### 🔌 Modos de Operação das Portas

- **Access Mode**: Portas conectadas a dispositivos finais (PCs).
- **Trunk Mode**: Habilitadas para múltiplas VLANs nos links entre switches e roteador.

---

### 🔁 RSTP e Segurança de Portas

- **RSTP**: Redução de tempo de convergência da rede em falhas.
- **Portfast** e **BPDU Guard**: Aplicadas às interfaces conectadas aos dispositivos finais para evitar loops.

---

### 📶 Router-on-a-Stick + DHCP

- Configuração de sub-interfaces no roteador R1 para rotear entre VLANs.
- DHCP configurado em pools separados para cada VLAN, fornecendo endereçamento automático para hosts.

---

### 🧭 Endereçamento IP

- **IPv4**: Endereçamento estático nas sub-interfaces do R1 e dinâmico via DHCP para PCs.
- **IPv6**: Sub-interfaces do R1 configuradas com IPv6 estático; hosts obtêm endereços via SLAAC.

---

## 📂 Arquivos Disponíveis

| Tipo | Arquivo | Descrição |
|------|---------|-----------|
| 📦 Cenário Packet Tracer | [Avaliação.pkt](https://github.com/joseffermax/Configura-o-Avancada-de-Redes-LAN-VLANs-LACP-e-Roteamento-Inter-VLAN/blob/main/Avalia%C3%A7%C3%A3o%20Tecnologias%20de%20Redes%20Locais.pkt) | Arquivo de topologia pronto para simulação |
| 📄 Documentação | [Instruções.pdf](https://github.com/joseffermax/Configura-o-Avancada-de-Redes-LAN-VLANs-LACP-e-Roteamento-Inter-VLAN/blob/main/Avalia%C3%A7%C3%A3o%20Tecnologias%20de%20Redes%20Locais.pdf) | Guia completo com as configurações utilizadas |

---

## 💻 Requisitos

- [Cisco Packet Tracer](https://www.netacad.com/)

> ⚠️ **Nota:** É necessário criar uma conta gratuita na Cisco Networking Academy para baixar e utilizar o simulador.

---

## 🛠️ Tecnologias Utilizadas

- Cisco Packet Tracer (Simulador)
- Protocolo LACP
- RSTP / Portfast / BPDU Guard
- VLANs, Subinterfaces, DHCP
- IPv4 / IPv6
- Router-on-a-Stick

---

## 🤝 Contribuições

Contribuições são bem-vindas! Caso tenha sugestões, melhorias ou correções, fique à vontade para abrir uma *issue* ou enviar um *pull request*.

---

## 📜 Licença

Distribuído sob a Licença MIT. Veja `LICENSE` para mais informações.

---

## 👨‍🏫 Orientação

Projeto desenvolvido sob orientação do professor **Marcelo Portela Sousa**, na disciplina de **Tecnologias de Redes Locais**.

---

## 📬 Contato

📧 Email: [joseffermax1472@gmail.com](mailto:joseffermax1472@gmail.com)  
🔗 GitHub: [@joseffermax](https://github.com/joseffermax)

---

<h2 align="center">🌐 Explore a topologia, aplique o conhecimento e domine as redes locais! 🚀</h2>
