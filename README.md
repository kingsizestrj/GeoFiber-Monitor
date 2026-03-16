# 🚀 GeoFiber Monitor | NOC Dashboard Pro

O **GeoFiber Monitor** é uma solução profissional de monitoramento georreferenciado para infraestruturas de rede e TI. Integrado nativamente ao **Zabbix**, ele permite visualizar o status de POPs e enlaces diretamente em um mapa interativo, transformando dados técnicos em inteligência visual para o seu NOC.

---

## 🛠️ Funcionalidades Principais

* **Mapa Interativo:** Visualização via Leaflet com suporte a importação de KML e desenho manual de rotas.
* **Monitoramento em Tempo Real:** Integração via API do Zabbix para leitura de Triggers e Itens de tráfego.
* **Alertas Visuais e Sonoros:** Animações de pulsação em elementos com falha e alertas sonoros.
* **Gestão de Backup:** Interface simplificada para download e restauração da base de dados da rede.
* **NOC Mode:** Interface limpa e otimizada para Video Walls e operação 24/7.
* **Segurança Industrial:** Backend criptografado e licenciamento vinculado ao hardware (HWID).

---

## 📦 Como fazer o Deploy (Instalação)

Este software é distribuído via Docker para garantir máxima estabilidade e isolamento.

### 1. Preparação do Servidor
Certifique-se de que o **Docker** e o **Docker Compose** estão instalados no servidor Linux (Ubuntu 22.04 LTS ou superior recomendado).

### 2. Deploy

```bash
git clone https://github.com/kingsizestrj/GeoFiber-Monitor.git

cd GeoFiber-Monitor

docker compose up -d
```
### 1. 🔐 Primeiro Acesso e Ativação
O GeoFiber Monitor requer uma licença ativa vinculada ao hardware do servidor para funcionar.

Acesse o painel pelo navegador: http://IP-DO-SERVIDOR:8080.

A tela de bloqueio exibirá o seu HWID (Código de Hardware) exclusivo.

Copie este código e envie ao desenvolvedor para receber sua Chave de Ativação.

Cole a chave no campo indicado e clique em 🔓 Desbloquear Sistema.

### 2. ⚙️ Configurando a Integração Zabbix
No menu lateral, vá em Configurar Zabbix.

Informe a URL da API (ex: http://monitor.empresa.com.br/zabbix/api_jsonrpc.php).

Informe o API Token gerado no Zabbix (Administração > Usuários > Tokens).

Clique em Salvar. A partir de agora, ao editar um elemento no mapa, você poderá vincular Grupos, Hosts e Triggers do seu Zabbix.

### 3. 💾 Backup e Manutenção

Rotina de Backup: Recomendamos baixar o arquivo de backup regularmente através do botão "Download Backup" no painel de ferramentas.

Restauração: Para restaurar, utilize o botão "Restaurar Backup" e selecione o arquivo .json gerado anteriormente.

### 4. 📞 Suporte e Licenciamento
Para suporte técnico ou renovação de licenças, entre em contato:

Desenvolvedor: Syllas Gonçalves Silva

email: syllasgoncalvess@gmail.com
telegram: https://t.me/SyllasGS

Versão: 1.0.0-Release
