# 🧠🔊 Chaveiro Inteligente com Reprodução de Áudio e Exibição de Logo

Este projeto consiste em um **chaveiro inteligente** que, ao ser acionado por um botão, **reproduz o hino do São Paulo Futebol Clube** e **exibe o logo do time** em um display **OLED**.  
Desenvolvido com o **microcontrolador Raspberry Pi Pico W**, o sistema combina técnicas de **sistemas embarcados**, como **PWM** para reprodução de áudio e **I2C** para controle do display.

---

## ⚙️ Funcionalidades

- **Reprodução de Áudio:** o hino do São Paulo é reproduzido através de um buzzer, utilizando **PWM** para gerar as frequências das notas musicais.  
- **Exibição de Logo:** a logo do São Paulo é exibida em um **display OLED 128x64 pixels**.  
- **Multicore:** o projeto utiliza os dois núcleos do **Raspberry Pi Pico W**, permitindo que a música seja tocada no **Core 1**, enquanto o **Core 0** gerencia a exibição da logo e a leitura do botão.  
- **Portabilidade:** o sistema é **alimentado por bateria**, tornando-o portátil e ideal para uso como chaveiro.

---

## 🧩 Componentes Utilizados

- **Microcontrolador:** Raspberry Pi Pico W  
- **Display:** OLED 128x64 (comunicação I2C)  
- **Buzzer:** para reprodução do áudio  
- **Botão:** para acionar o sistema  
- **Bateria:** para alimentação do circuito  

---

## 🧠 Como Funciona

1. Ao pressionar o botão, o sistema detecta o acionamento e inicia a reprodução do hino.  
2. Simultaneamente, a logo do São Paulo é exibida no display OLED.  
3. O hino é reproduzido utilizando **PWM** para gerar as frequências correspondentes às notas musicais.  
4. Após a reprodução, o sistema retorna ao estado inicial, aguardando um novo acionamento.

---

## 🔌 Montagem do Circuito

| Componente       | Pino do Pico W          | Função                         |
|------------------|-------------------------|---------------------------------|
| **Buzzer**       | GP21                    | Saída PWM (áudio)              |
| **Botão**        | GP6                     | Entrada digital com pull-up    |
| **Display OLED** | GP14 (SDA), GP15 (SCL)  | Comunicação I2C                |

---

## 🎥 Vídeo de Demonstração

📺 [Assista ao vídeo no YouTube](https://youtube.com/shorts/UOWDGTUV_6g?feature=share) <!-- Substitua o "#" pelo link real -->

---

## 🤝 Contribuições

Contribuições são bem-vindas!  
Sinta-se à vontade para **abrir issues** ou **enviar pull requests** com sugestões e melhorias.

---

## 🪪 Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).

---

## 👨‍💻 Autor

**João Nogueira**  
🔗 [LinkedIn](https://www.linkedin.com/in/jo%C3%A3o-nogueira-5898902b2/)
