# Lista de Materiais e Softwares

## Hardware

- **ESP32-CAM** com câmera OV2640 (2MP)
  - Microcontrolador ESP32 com Wi-Fi e Bluetooth integrados
  - Câmera OV2640 de 2 megapixels
- **Programador FTDI** ou **ESP32-CAM MB** para upload do firmware
- **Fonte de alimentação USB** (5V, pelo menos 1A)
- **Cabos jumper** (para conexões entre ESP32-CAM e programador)
- **Protoboard** (opcional, para montagem e testes)
- **Suporte para câmera** (opcional, para fixação do módulo)
- **Caixa ou case protetora** (opcional, para acomodar o hardware)

## Software

### Para o ESP32-CAM

- **Arduino IDE** (recomendado: versão 1.8.18)
  - Pacote de placas ESP32 para Arduino IDE
  - Biblioteca ESP32 Camera
  - Bibliotecas adicionais:
    - `WiFi.h` (conexão Wi-Fi)
    - `HTTPClient.h` (requisições HTTP)
    - `esp_camera.h` (controle da câmera)
    - Bibliotecas de detecção facial (inclusas no exemplo CameraWebServer)

### Para o Servidor de Reconhecimento Facial

- **Python 3.8+**
- **Django** (framework web)
- **Biblioteca `face_recognition`** (processamento facial)
- **OpenCV** (manipulação de imagens)
- **NumPy** (processamento numérico)
- **Django REST Framework** (para criação de APIs RESTful)
- **Gunicorn** ou **uWSGI** (para deploy do servidor, opcional)
- **Nginx** ou **Apache** (para servir a aplicação em produção, opcional)

### Ferramentas de Desenvolvimento

- **Editor de código** (Visual Studio Code, PyCharm, etc.)
- **Git** (controle de versão)
- **Ferramentas para teste de API** (Postman, Insomnia)
- **ThinkerCad** (modelagem e simulação de protótipos)
- **Docker** (opcional, para facilitar o deploy e testes do servidor)

---

> **Observação:** Certifique-se de que todos os drivers do programador FTDI estejam instalados no sistema operacional utilizado.