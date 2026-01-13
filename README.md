# FMCW-DIY-Radar
Este projeto tem como objetivo projetar para estudo um Radar do tipo Frequency-modulated continuous-wave radar (FM-CW).

# Topologia
Este tipo de radar se baseada na transimssão continua de uma chirp de frequência. Um sinal modulado em uma rampa linear de frequência é transmitido. Sua reflexão é capturada, a distância é estimada através da diferência entre o sinal recebido e o que está sendo transmitido no instante.

![395890914-43e02710-3b98-4efa-8052-6310c8257413](https://github.com/user-attachments/assets/c54d740f-6812-4295-a88a-67309a75d88d)

# Especificações
Para este radar FMCW o objetivo é projetar um radar operando na faixa SHF na Banda C, especificamente na banda ISM, de 5,725GHz para 5,875GHz. O radar será um mono estático com antenas para transmissão e recepção separadas, para haver alto isolamento.

**Especificações objetivos:**

- Medir distancia e velocidade
- $d_{max}\gt100m$ para alvos com $\sigma=1$  (aproximadamente de um humano adulto)
- $v_{max}\ge15m/s$
- microcontrolador ARM capaz de realizar todo processamento necessário.
- Display LCD para exibição dos resultados.
- PCB de 2/4 camadas feita pela JLCPCB de máximo 100mmx100mm para os circuitos de RF
- PCB de 4 camadas feita pela JLCPCB de máximo 100mmx100mm para os circuitos digitais
- Alimentado pelo USB-C.
- Transferência dos dados brutos para o computador.
- Visualização por interface gráfica em MATLAB ou programa escrito em Julia/Python

# Projeto

# Placa Digital
https://365.altium.com/files/D23D9574-CF08-4959-81D4-2C4755ACD176)

A placa digital contém os circuitos digitais e de banda base do radar. O microcontrolador, conversores A/D e D/A, filtros, conexão e alimentação.

<img width="2339" height="1653" alt="Radar-1" src="https://github.com/user-attachments/assets/1db06763-b03b-4de5-92c2-da6e0740ae34" />

A PCB de 85mm x 65mm possuí 4 camadas de cobre com a seguinte configuração: SIG/PWR - GND - GND - SIG/PWR:

<img width="1036" height="725" alt="image" src="https://github.com/user-attachments/assets/aae8a137-6b0d-4c14-b303-46b497cd29e8" />
<img width="1109" height="784" alt="image" src="https://github.com/user-attachments/assets/4a88a06b-a33d-429c-a15a-8a2711083ccf" />

# Referências
https://en.wikipedia.org/wiki/Continuous-wave_radar

https://hforsten.com/third-version-of-homemade-6-ghz-fmcw-radar.html

https://www.youtube.com/@MarshallBrunerRF
