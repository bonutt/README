
🌊 Projeto IoT: Monitoramento de Enchentes Urbanas

Este projeto simula uma solução de Internet das Coisas (IoT) para **detecção precoce de enchentes** em áreas urbanas críticas, utilizando sensores, automação e dashboards em tempo real.

🎯 Problema

Enchentes urbanas causam prejuízos materiais, bloqueios em vias públicas e colocam vidas em risco. A detecção precoce é essencial para alertar moradores e autoridades antes que os alagamentos se agravem.

✅ Solução Proposta

O sistema utiliza sensores conectados a um ESP32, que monitora:

- Nível da água
- Temperatura do ambiente
- Umidade relativa do ar

Com esses dados, o sistema decide automaticamente se há risco de enchente e aciona alertas visuais (LED) e sonoros (buzzer). Os dados também são enviados para um dashboard acessível remotamente via navegador.

🧱 Arquitetura da Solução

📡 1. Camada IoT (Dispositivos e Sensores)

- **ESP32 (Wokwi)**: microcontrolador principal
- **Sensor HC-SR04**: mede a distância da superfície da água
- **Sensor DHT22**: mede temperatura e umidade
- **LED e Buzzer**: atuadores que disparam em situações críticas

🔁 2. Camada Back-End (Lógica e Comunicação)

- **Node-RED** (FlowFuse ou FRED)
- **Bloco `function`**: aplica a lógica de alerta
- **MQTT (simulado)**: protocolo para transmitir dados de sensores

🖥️ 3. Camada de Aplicação (Dashboard Web)

- **Node-RED Dashboard (`/ui`)**
  - `ui_gauge`: exibe temperatura
  - `ui_gauge`: exibe umidade
  - `ui_chart`: mostra gráfico do nível da água
  - `ui_text`: alerta textual sobre risco de enchente

🔗 Links

- 🔧 **Projeto Wokwi (Simulação do ESP32)**: [Clique aqui](https://wokwi.com/projects/432983265256290305)
- 📊 **Dashboard Node-RED (via FlowFuse/FRED)**: [Insira o link real do seu painel `/ui` aqui]

🚀 Como Executar

1. Wokwi
- Acesse o link do projeto Wokwi
- Clique em **“Start Simulation”**
- Veja os dados sendo atualizados no Serial Monitor

2. Node-RED
- Acesse o editor Node-RED
- Clique em **Deploy**
- Acesse `/ui` para visualizar o dashboard em tempo real

👨‍💻 Tecnologias Utilizadas

- ESP32 (simulado)
- Sensores DHT22 e HC-SR04
- Node-RED + Node-RED Dashboard
- MQTT (simulado)
- Wokwi + FlowFuse (ou FRED)

📷 Imagens do Projeto
![image](https://github.com/user-attachments/assets/59eed21c-92d4-44a5-a525-b8bfa6a437e7)



Créditos
Projeto desenvolvido por Luigi bonuccelli rm 560950.

