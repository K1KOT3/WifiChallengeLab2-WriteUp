# WifiChallengeLab2 - Seguridad en Redes Inalámbricas

📡 **Análisis de seguridad WiFi mediante ataques de reconocimiento, autenticación y cracking de contraseñas**  

Este repositorio contiene el informe del **WifiChallengeLab 2.1**, donde se realizaron diversas pruebas de seguridad en redes inalámbricas, explorando técnicas de **Reconnaissance (Recon), Open Networks (OPN) y Pre-Shared Key (PSK)**.

## 🔍 Descripción

El objetivo de este laboratorio es analizar vulnerabilidades en redes WiFi, identificar posibles fallos de seguridad y poner en práctica métodos de auditoría en redes inalámbricas, incluyendo:
- **Captura de tráfico y análisis con Airodump-ng y Wireshark**.
- **Bypass de autenticación en redes abiertas** mediante suplantación de MAC.
- **Ataques de fuerza bruta y cracking de contraseñas WPA/WPA2** utilizando `aircrack-ng` y `hashcat`.
- **Uso de cookies de sesión y ataques man-in-the-middle (MITM)** para autenticaciones web en redes WiFi.

## 📁 Contenido del Repositorio

- `WifiChallengeLab2_EnriqueGarciaCuadrado.pdf` → Informe completo con técnicas y resultados.
- Scripts y comandos utilizados en la auditoría WiFi (pendiente de añadir).

## 🛠 Herramientas Utilizadas

### 🔹 **Fase de Reconocimiento (Recon)**
- **Airodump-ng** → Captura de tráfico WiFi y detección de redes disponibles.
- **Fuerza bruta sobre handshakes** → Cracking de WPA2 con `aircrack-ng` y diccionarios (`rockyou-top100000.txt`).

### 🔹 **Fase de Redes Abiertas (OPN)**
- **Suplantación de MAC** → Bypass de autenticación en redes sin cifrado.
- **Interceptación de tráfico HTTP con Wireshark**.
- **Uso de `curl` para autenticación con cookies de sesión**.

### 🔹 **Fase de Redes Protegidas (PSK)**
- **Ataques de desautenticación con Aireplay-ng** → Captura de handshakes WPA2.
- **Descifrado de tráfico con Airdecap-ng**.
- **Ataques de punto de acceso falso para captura de credenciales**.

## 🚀 Hallazgos Destacados

- **Compromiso de credenciales en redes WiFi abiertas** mediante interceptación de tráfico.
- **Vulnerabilidades en redes WPA2** por ataques de fuerza bruta y recolección de handshakes.
- **Evasión de restricciones de acceso** en entornos WiFi con autenticación basada en cookies.
- **Falta de aislamiento de clientes WiFi** permitiendo ataques MITM y escaneo de red interna.

