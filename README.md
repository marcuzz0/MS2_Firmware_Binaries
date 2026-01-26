# MS2 Firmware

## Aggiornamento OTA (via WiFi)

1. Connetti MS2 a una rete WiFi
2. Menu → **Update Firmware** → **Check for device firmware**
3. Se disponibile una nuova versione, seleziona **Update**

## Aggiornamento da SD Card

1. Scarica il file `.bin` dalla tabella sopra
2. Copia il file sulla SD card (root)
3. Inserisci la SD nel dispositivo
4. Menu → **Update Firmware** → Seleziona il file

## Aggiornamento via Seriale (USB)

### Con esptool.py

1. Installa esptool: `pip install esptool`
2. Collega MS2 via USB
3. Esegui:
```bash
esptool.py --chip esp32 --port /dev/ttyUSB0 --baud 921600 write_flash 0x10000 MS2_Firmware_v1_0.bin
```
(Su Windows usa `COM3` o la porta appropriata)

### Con Arduino IDE

1. Apri Arduino IDE
2. Seleziona **Tools** → **Board** → **ESP32 Dev Module**
3. Seleziona la porta seriale corretta
4. **Sketch** → **Upload Compiled Binary** → Seleziona il file `.bin`

## Force Update

Per forzare l'aggiornamento all'avvio:
1. Rinomina il file in `MS2_Firmware_Force.bin`
2. Copia sulla SD card
3. Riavvia il dispositivo
