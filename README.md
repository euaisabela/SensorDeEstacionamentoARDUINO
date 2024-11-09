# Projeto de Estacionamento Inteligente com Arduino e Sensor Ultrassônico

Este projeto é uma solução simples para monitoramento de vagas de estacionamento usando sensores ultrassônicos, LEDs e um buzzer, desenvolvida com a plataforma Arduino. O objetivo é verificar a disponibilidade de vagas e indicar se estão livres ou ocupadas. O sistema também emite um som (buzzer) quando o sensor detecta um carro se aproximando da vaga.

## Descrição do Projeto

O projeto usa dois sensores ultrassônicos para medir a distância até o veículo e determina se a vaga está ocupada ou livre com base na distância medida. A seguir, são acesos LEDs verdes ou vermelhos para indicar o estado das vagas. Um buzzer emite um som alto quando um carro está se aproximando, e o som para quando a vaga é ocupada.

## Componentes Utilizados

- **Placa Arduino (Uno ou compatível)**
- **2 Sensores Ultrassônicos (HC-SR04)**
- **2 LEDs Vermelhos**
- **2 LEDs Verdes**
- **1 Buzzer**
- **Fios de Conexão**
- **Protoboard (opcional)**
- A BATERIA ( utilizamos uma carregador portátil) 

## Diagrama de Conexões

### Sensor Ultrassônico 1 (Vaga 1):
- **Trig**: Pino 9
- **Echo**: Pino 10

### Sensor Ultrassônico 2 (Vaga 2):
- **Trig**: Pino 11
- **Echo**: Pino 12

### LEDs:
- **LED Vermelho Vaga 1**: Pino 7
- **LED Verde Vaga 1**: Pino 6
- **LED Vermelho Vaga 2**: Pino 5
- **LED Verde Vaga 2**: Pino 4

### Buzzer:
- **Pino do Buzzer**: Pino 8

## Funcionamento

1. **Leitura dos Sensores Ultrassônicos**:
   - O sistema lê a distância dos sensores ultrassônicos a cada 100 ms. Quando a distância medida é menor que 6 cm, a vaga é considerada **ocupada**.
   - Se a distância estiver entre 7 e 10 cm, o **buzzer** é acionado para alertar a presença de um veículo.

2. **Controle dos LEDs**:
   - **LED Vermelho** acende quando a vaga está ocupada.
   - **LED Verde** acende quando a vaga está livre.

3. **Buzzer**:
   - O buzzer emite um som quando o sensor detecta que o carro está se aproximando da vaga (distância entre 7 e 10 cm).
   - O som é interrompido quando a vaga está ocupada (distância menor que 6 cm).

## Código

O código do projeto pode ser encontrado no arquivo `main.ino`. Ele inclui a configuração dos pinos do Arduino, a leitura dos sensores ultrassônicos, o controle dos LEDs e do buzzer.










ALGUMAS IMAGENS INICIAIS DE COMO SERIA INSTALADO NO PROEJETO FÍSICO:

LINK DO SITE : https://www.tinkercad.com/

![image](https://github.com/user-attachments/assets/5ceb8d08-1b88-4dfb-ba77-bf7133cff024)


![image](https://github.com/user-attachments/assets/eadecf53-7a28-4c02-9926-21222ac6f333)

