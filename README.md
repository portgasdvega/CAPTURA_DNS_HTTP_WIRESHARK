# ANALISIS DE DNS Y HTTP EN WIRESHARK

# Análisis de Tráfico DNS y HTTP con Wireshark

Este repositorio contiene una práctica básica de análisis de tráfico de red usando Wireshark, enfocada en los protocolos DNS y HTTP. Esta actividad demuestra la capacidad para interpretar estructuras de paquetes y el comportamiento de las solicitudes/respuestas en la red.

---

## Objetivo

Capturar e interpretar tráfico real de red asociado a los protocolos:

- **DNS (Domain Name System)**
- **HTTP (HyperText Transfer Protocol)**

Usando la herramienta Wireshark para comprender cómo se resuelven nombres de dominio y cómo se solicita contenido web.

---

## Herramientas

- Wireshark
- Sistema operativo Kali Linux
- Terminal con `curl` y `ping`

---

## Captura

Se utilizaron los siguientes comandos para generar tráfico:

```bash
ping example.com
curl http://example.com

El filtro aplicado en Wireshark fue:
tcp.port == 80 || udp.port == 53
