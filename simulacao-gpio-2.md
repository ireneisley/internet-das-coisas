# Código 2 – Controle por PWM e Interrupções

<p align="justify">
Este projeto corresponde ao <strong>Código 2 da atividade de GPIOs</strong> da disciplina de <strong>Internet das Coisas</strong> do <strong>IFPB</strong>. A simulação foi desenvolvida utilizando o microcontrolador <strong>ESP32-C6</strong> no simulador <strong>Wokwi</strong>, com o objetivo de demonstrar o uso de <strong>PWM</strong>, além da utilização de interrupções por GPIO, temporizador e comunicação serial, permitindo que o sistema reaja a diferentes eventos externos.
</p>

## Funcionamento

<p align="justify">
O sistema utiliza <strong>4 LEDs, 2 botões e 1 buzzer conectados ao ESP32-C6</strong>, explorando o uso do periférico <strong>LEDC</strong> para geração de sinais PWM e interrupções para resposta a eventos.
</p>

- **Fading dos LEDs:**  
  Os LEDs variam suavemente o brilho de **0% a 100%**, retornando gradualmente ao valor inicial.

- **Som variável no buzzer:**  
  O buzzer emite um som cuja frequência varia gradualmente de **500 Hz até 2 kHz**, retornando em seguida à frequência inicial.

- **Botão A:**  
  Quando pressionado, alterna o estado do **LED1**.

- **Botão B:**  
  Quando pressionado, ativa o **buzzer por 1,5 segundos**.

- **Timer:**  
  Um temporizador interno alterna automaticamente o **LED2 a cada 2 segundos**.

- **Comunicação UART:**  
  Pela interface serial, é possível enviar comandos:
  - `a` → desativa o botão B  
  - `b` → reativa o botão B  

## Simulação

<p align="justify">
Acesse a simulação no Wokwi pelo link abaixo:
</p>

🔗 https://wokwi.com/projects/457692694275435521

## Componentes Utilizados

- ESP32-C6  
- 💡 4 LEDs  
- 2 Botões  
- Buzzer piezoelétrico  
- Resistores  
- GPIOs configuradas como entrada, saída e PWM  
