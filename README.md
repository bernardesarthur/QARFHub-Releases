<p align="center">
  <img src="logo.png" alt="Quero Automação — QA RF Hub" width="300">
</p>

# QA RF Hub — Downloads

Página oficial de downloads dos firmwares do sistema **QA RF Hub** da [Quero Automação](https://github.com/queroautomacao).

📦 **Para baixar a versão mais recente:** [Releases](https://github.com/queroautomacao/QARFHub-Releases/releases/latest)

## 🟢 Hub RF (QARFHub)

Firmware do controlador principal — Somfy RTS + controles RF de protocolo aberto.

**Arquivos:**
- `QARFHub.ino.bin` — firmware (atualiza app + funcionalidades)
- `QARFHub.ino.littlefs.bin` — WebUI (atualiza interface)
- `QARFHub-Update-vX.Y.Z.zip` — pacote com ambos + LEIA-ME

**Como atualizar:**

1. Conecte na WebUI da placa pelo IP local
2. Vá em **System → Firmware → Update Firmware**
3. Faça os 2 uploads em sequência (qualquer ordem — o dispositivo detecta automaticamente):
   - `QARFHub.ino.bin`
   - `QARFHub.ino.littlefs.bin`
4. Aguarde ~20s entre uploads para a placa reiniciar
5. Após o segundo upload, verifique a versão no rodapé da WebUI

> ⚠️ **Para placas com firmware ≤ v1.4.2:** o nome do arquivo precisa conter `.ino.` para passar pela validação antiga. Renomeie `QARFHub.littlefs.bin` para `QARFHub.ino.littlefs.bin` antes do upload (já vem com esse nome nas releases v1.5.0+).

## 🔵 Cubo Tuya (QARF8)

Firmware do bridge que conecta o QARFHub à nuvem Tuya.

**Arquivo:**
- `QARF8_QIO_X.Y.Z.bin` — firmware completo (flash inicial via USB)

**Atualização normal: automática via Tuya OTA**
Se a placa já está pareada e online no app Tuya, ela recebe a atualização sozinha em até 24h. Não precisa fazer nada.

Se em 24h a atualização não aparecer, envie o **Device ID** ao suporte:
1. App Tuya → toque no dispositivo
2. Ícone de lápis ✏️ no canto superior direito
3. **Informações do dispositivo** → copie o **Virtual ID**
4. Envie ao nosso suporte para liberação manual

## 🔌 Hardware

- **Placa:** ESP32-S3 DevKitC-1 N16R8 (16 MB flash, 8 MB PSRAM)
- **Rádio:** CC1101 433 MHz

## 🏠 Integração com Home Assistant

Repositório separado: https://github.com/queroautomacao/QARFHub-HA

Instalação via HACS como repositório customizado.

## 💬 Suporte

Em caso de dúvidas ou problemas, entre em contato pelo canal oficial da Quero Automação.
