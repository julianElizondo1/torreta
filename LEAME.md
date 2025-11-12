# 🌍 Proyecto: Terra 3D

**Terra 3D** es una torreta automática desarrollada con **Arduino UNO**, capaz de detectar objetos mediante un **sensor ultrasónico HC-SR04** y reaccionar con una **señal sonora**.  
El sistema utiliza un **motor paso a paso 28BYJ-48** (con driver ULN2003) para girar su cabeza en un rango aproximado de **90°**, escaneando el entorno constantemente.  

Cuando el sensor detecta un objeto a menos de cierta distancia, la torreta se **detiene momentáneamente** y emite **tres pitidos cortos** con el buzzer antes de continuar su patrullaje.

> 💡 En futuras versiones se prevé incorporar un **LED de alerta visual** para complementar la respuesta sonora del sistema.

---

## ⚙️ Componentes utilizados

- 🧠 **Arduino UNO**  
- 🔄 **Motor paso a paso 28BYJ-48** + **driver ULN2003**  
- 📏 **Sensor ultrasónico HC-SR04**  
- 🔊 **Buzzer piezoeléctrico**  
- 🔌 **Protoboard y cables de conexión**

---

## 🔌 Conexiones principales

| Componente | Pin Arduino | Descripción |
|-------------|-------------|--------------|
| HC-SR04 Trig | D5 | Disparo de la señal ultrasónica |
| HC-SR04 Echo | D6 | Recepción del eco (medición de distancia) |
| Buzzer (+) | D3 | Alerta sonora (tres pitidos cortos) |
| ULN2003 IN1–IN4 | D8–D11 | Control del motor paso a paso |
| 5V y GND | — | Alimentación común |

---

## 💻 Software

- 💬 Desarrollado en **Arduino IDE**  
- 🔠 Lenguaje: **C++ para Arduino**  
- 📚 Librería utilizada: [`Stepper.h`](https://www.arduino.cc/en/reference/stepper)

---

## 🚀 Funcionamiento

1. La torreta realiza un **movimiento de patrulla** girando de un lado a otro (≈90°).  
2. El **sensor ultrasónico HC-SR04** mide constantemente la distancia frente a la torreta.  
3. Si detecta un objeto a menos de la distancia configurada (por ejemplo, 20 cm):  
   - 🛑 La torreta se **detiene**.  
   - 🔊 Emite **tres pitidos cortos** de alerta.  
   - 🔁 Luego **reanuda su movimiento normal**.  

---

## 🔮 Futuras mejoras

El diseño de **Terra 3D** puede evolucionar incorporando nuevas características:

- 💡 **Indicador LED de alerta visual**.  
- 📱 **Notificaciones al celular** mediante Bluetooth o WiFi al detectar objetos.  
- 🎯 **Control remoto o seguimiento dinámico de objetivos**.  
- 📷 **Integración con cámaras o sensores adicionales**.  

Estas mejoras buscan transformar la maqueta actual en un **sistema más completo de vigilancia o demostración tecnológica**.

---

## 📸 Presentación

El proyecto puede integrarse en una **maqueta física**, donde la base aloja la electrónica y la “cabeza” móvil simula una cámara o sensor activo.  
Ideal como **proyecto educativo** sobre robótica, sensores y control de motores paso a paso, destacando el uso combinado de hardware accesible y programación en Arduino.

---

## 🧩 Autores

**Julian Elizondo**  y **Dylan Del Rio**
Proyecto desarrollado como parte de una práctica de robótica y sistemas embebidos.  
📅 *Versión actual: noviembre 2025*

