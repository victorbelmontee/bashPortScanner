# 🌐 Bash Port Scanner

![License](https://img.shields.io/badge/license-MIT-blue.svg)  
![Bash Version](https://img.shields.io/badge/bash-4.0%2B-green.svg)  
![Platform](https://img.shields.io/badge/platform-Linux%20%7C%20macOS-lightgrey.svg)  
![Network](https://img.shields.io/badge/tool-Network%20Scanner-red.svg)  

Escáner de puertos en Bash que recorre el rango 1–65535 y detecta puertos TCP abiertos.

---

## 📋 Tabla de Contenidos

- [🚀 Características Principales](#-características-principales)  
- [📦 Instalación](#-instalación)  
- [💡 Uso](#-uso)  
- [📊 Ejemplos de Uso](#-ejemplos-de-uso)  
- [🤝 Contribución](#-contribución)  
- [📄 Licencia](#-licencia)  

---

## 🚀 Características Principales

- **Escaneo Completo**: Revisa puertos 1–65535  
- **Conexión Nativa**: Usa `/dev/tcp` para chequear apertura  
- **Concurrencia**: Lanza comprobaciones en background para velocidad  
- **Salida Limpia**: Muestra sólo puertos abiertos  
- **Manejo de Señales**: Captura Ctrl+C y restaura cursor  

---

## 📦 Instalación

> **Requisitos**  
> - Bash 4.0+  
> - Permiso de red saliente  
> - `tput` disponible  

```bash
git clone https://github.com/victorbelmontee/bashPortScanner.git
cd bashPortScanner
chmod +x portScan.sh
```

---

## 💡 Uso

```bash
# Escanear host (por ejemplo 192.168.1.10)
./portScan.sh 192.168.1.10
```

---

## 📊 Ejemplos de Uso

```bash
# Ejecutar en segundo plano
./portScan.sh 10.0.0.5 &

# Filtrar salida con grep
./portScan.sh 192.168.1.100 | grep OPEN
```

---

## 🤝 Contribución

Sigue el flujo estándar de Fork → Branch → Commit → PR.

---

## 📄 Licencia

MIT. Ver [`LICENSE`](LICENSE).
