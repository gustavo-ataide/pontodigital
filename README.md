# Sistema de Reconhecimento Facial com ESP32-CAM

## Descrição do Projeto

Este projeto consiste em um sistema de reconhecimento facial utilizando o módulo **ESP32-CAM**. O objetivo é detectar faces localmente no ESP32-CAM e enviar as imagens capturadas para um servidor externo, onde será realizado o reconhecimento facial mais complexo. O ESP32-CAM é responsável pela captura de imagens e detecção básica de faces, enquanto o processamento pesado de reconhecimento e comparação é feito por um servidor dedicado.

A solução é ideal para aplicações como controle de ponto, realização de chamadas de presença escolares e liberação de entrada de moradores em condomínios, aproveitando uma abordagem híbrida: detecção local + reconhecimento remoto, contornando as limitações de processamento do ESP32-CAM.

---

## Funcionalidades

- **Captura de Imagens:** Utiliza a câmera OV2640 do ESP32-CAM para capturar imagens.
- **Detecção de Faces:** Detecta faces em tempo real nas imagens capturadas.
- **Transmissão de Imagens:** Envia imagens para um servidor remoto quando uma face é detectada.
- **Interface Web:** Permite visualização do streaming de vídeo e ajuste de configurações da câmera.
- **Ajustes de Câmera:** Suporte para configuração de qualidade, brilho, contraste, saturação, etc.
- **Indicação Visual:** Desenha caixas ao redor das faces detectadas.
- **Processamento no Servidor:** O servidor realiza o reconhecimento facial e retorna os resultados.
- **Cadastro de Faces:** Permite cadastrar faces conhecidas no servidor para reconhecimento futuro.

---

## Requisitos

### Funcionais

1. Captura de imagens pela câmera OV2640.
2. Detecção de faces em tempo real.
3. Envio das imagens ao servidor remoto.
4. Interface web para visualização e configuração.
5. Ajuste de parâmetros da câmera.
6. Feedback visual na detecção de faces.
7. Processamento de reconhecimento facial no servidor.
8. Cadastro de faces conhecidas.

### Não Funcionais

1. Detecção em tempo real (latência < 10 segundos).
2. Estabilidade e recuperação automática em caso de falhas.
3. Comunicação segura entre ESP32-CAM e servidor.
4. Interface web intuitiva e responsiva.
5. Eficiência energética.
6. Alta precisão na detecção facial.

---

## Materiais e Ferramentas

### Hardware

- **ESP32-CAM** com câmera OV2640
- Programador FTDI ou ESP32-CAM MB para upload do código
- Fonte de alimentação USB

### Software

- **Arduino IDE** (recomendado: 1.8.18)
  - Pacote ESP32 para Arduino IDE
  - Biblioteca ESP32 Camera
- **Servidor para reconhecimento facial**
  - Python + Django
  - Biblioteca `face_recognition`
  - OpenCV
  - NumPy
- **Bibliotecas adicionais para ESP32**
  - WiFi.h, HTTPClient.h, esp_camera.h
  - Bibliotecas de detecção facial (inclusas no exemplo CameraWebServer)
- **Ferramentas de desenvolvimento**
  - Editor de código (VS Code, PyCharm, etc.)
  - Git
  - Ferramentas de teste de API (Postman, Insomnia)
- **Modelagem do protótipo**
  - ThinkerCad

---

## Como Usar

1. **Monte o hardware** conforme a lista de materiais.
2. **Configure o Arduino IDE** e faça upload do código para o ESP32-CAM.
3. **Configure o servidor** Python/Django para receber e processar as imagens.
4. **Acesse a interface web** para visualizar o streaming e ajustar configurações.
5. **Cadastre faces** conhecidas via interface do servidor.

---

## Observações

- O reconhecimento facial completo é feito no servidor, não no ESP32-CAM.
- Recomenda-se utilizar uma rede Wi-Fi estável para comunicação entre ESP32-CAM e servidor.
- Para melhor desempenho, utilize um servidor com boa capacidade de processamento e memória.
