# Requisitos Não Funcionais

1. **Desempenho e Latência**
   - O sistema deve realizar a detecção de faces e o envio das imagens ao servidor em tempo real, com latência máxima de 10 segundos entre a captura e o retorno do resultado do reconhecimento facial.

2. **Confiabilidade e Robustez**
   - O sistema deve operar de forma estável, com mecanismos automáticos de recuperação em caso de falhas de hardware, software ou comunicação, minimizando períodos de indisponibilidade.

3. **Segurança**
   - Toda comunicação entre o ESP32-CAM e o servidor deve ser protegida por protocolos seguros (como HTTPS/TLS), garantindo a confidencialidade e integridade dos dados transmitidos.
   - O acesso à interface web e às APIs deve ser autenticado e autorizado, protegendo dados sensíveis e funcionalidades administrativas.

4. **Usabilidade e Acessibilidade**
   - A interface web deve ser intuitiva, responsiva e acessível em diferentes dispositivos (desktop, tablet, smartphone), facilitando a configuração e o monitoramento do sistema por usuários de diferentes perfis.

5. **Eficiência Energética**
   - O sistema deve otimizar o consumo de energia do ESP32-CAM, utilizando modos de baixo consumo quando possível e evitando processamento desnecessário.

6. **Precisão e Qualidade**
   - Os algoritmos de detecção e reconhecimento facial devem apresentar alta taxa de acerto, minimizando falsos positivos e falsos negativos, e garantindo a confiabilidade dos resultados.

7. **Escalabilidade**
   - O sistema deve ser projetado para permitir a adição de múltiplos dispositivos ESP32-CAM e a expansão do servidor para suportar aumento de demanda sem degradação significativa de desempenho.

8. **Manutenibilidade**
   - O código-fonte e a arquitetura do sistema devem ser documentados e estruturados para facilitar manutenção, atualização e evolução futura.

9. **Compatibilidade**
   - O sistema deve ser compatível com diferentes navegadores web modernos e sistemas operacionais, garantindo ampla acessibilidade.

10. **Monitoramento e Auditoria**
    - O sistema deve fornecer mecanismos de monitoramento de desempenho, geração de logs e auditoria de eventos relevantes para facilitar a identificação e resolução de de problemas.

---