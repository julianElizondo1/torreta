# 🌍 Proyecto: Terra 3D

**Terra 3D** es una torreta automática desarrollada con **Arduino UNO**, capaz de detectar movimiento y reaccionar de forma visual y sonora.  
El sistema utiliza un **sensor PIR** para identificar presencia, un **motor paso a paso 28BYJ-48** (con driver ULN2003) para girar su cabeza en un rango de unos 90°, y un conjunto de **LED y buzzer** para indicar detección de movimiento.  

Cuando la torreta detecta algo, se detiene momentáneamente, enciende su LED de alerta y emite tres pitidos cortos, antes de continuar su patrullaje normal.

---

## ⚙️ Componentes utilizados
- Arduino UNO  
- Motor paso a paso **28BYJ-48** + **driver ULN2003**  
- Sensor de movimiento **PIR HC-SR501**  
- LED rojo + resistencia de 220 Ω  
- Buzzer piezoeléctrico  
- Protoboard y cables de conexión  

---

## 🔌 Conexiones principales

| Componente | Pin Arduino | Descripción |
|-------------|-------------|-------------|
| PIR (OUT) | D2 | Señal de movimiento |
| LED (+) | D3 | Indicador de alerta |
| Buzzer (+) | D4 | Pitidos de aviso |
| ULN2003 IN1–IN4 | D8–D11 | Control del motor |
| 5V y GND | — | Alimentación común |

---

## 💻 Software
- Desarrollado en el **Arduino IDE**  
- Lenguaje: **C++ para Arduino**  
- Librería utilizada: [`Stepper.h`](https://www.arduino.cc/en/reference/stepper)

---

## 🚀 Funcionamiento
1. La torreta realiza un movimiento continuo de un lado a otro (≈90°).  
2. Si el sensor PIR detecta movimiento:
   - La torreta se detiene.  
   - Se enciende el LED y suenan tres pitidos cortos.  
   - Luego continúa su recorrido normal.  

---

## 🔮 Futuras mejoras
El diseño de **Terra 3D** tiene potencial para incorporar nuevas funciones, como:
- Envío de **notificaciones al celular** mediante Bluetooth o WiFi cuando se detecte movimiento.  
- Control remoto o seguimiento de objetivos.  
- Integración con cámaras o sensores adicionales.  

Estas mejoras buscan transformar la maqueta actual en un sistema más completo de monitoreo o demostración tecnológica.

---

## 📸 Presentación
El proyecto puede integrarse en una maqueta donde la base contiene la electrónica y la “cabeza” móvil simula una cámara o sensor.  
Es ideal como **proyecto educativo** sobre robótica, sensores y control de motores paso a paso.

---

## 📄 Autor
Proyecto **Terra 3D** desarrollado por **[Dylan Del Rio y Julián Elizondo]**, utilizando una placa **Arduino UNO** y componentes básicos fácilmente disponibles.
