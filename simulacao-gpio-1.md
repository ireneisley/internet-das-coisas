# Código 1 – Controle Digital de LEDs

<p align="justify">
Este projeto corresponde ao <strong>Código 1 da atividade de GPIOs</strong> da disciplina de <strong>Internet das Coisas</strong> do <strong>IFPB</strong>. A simulação foi desenvolvida utilizando o microcontrolador <strong>ESP32-C6</strong> no simulador <strong>Wokwi</strong>, com o objetivo de demonstrar o controle de saídas digitais por meio de GPIOs.
</p>

## Funcionamento

<p align="justify">
O sistema utiliza 4 LEDs conectados às GPIOs do ESP32-C6 e apresenta duas etapas de funcionamento:
</p>

- **Fase 1 – Contador Binário:**  
  Os LEDs representam valores binários de **0 a 15**, atualizando a cada **500 ms**.

- **Fase 2 – Sequência de Varredura:**  
  Os LEDs acendem sequencialmente **(LED1 → LED4)** e depois retornam **(LED4 → LED1)**, criando um efeito de varredura.

## Simulação

<p align="justify">
Acesse a simulação no Wokwi pelo link abaixo:
</p>

🔗 https://wokwi.com/projects/457663404169704449

## Componentes Utilizados

- ESP32-C6  
- 4 LEDs  
- Resistores  
- GPIOs configuradas como saída digital
