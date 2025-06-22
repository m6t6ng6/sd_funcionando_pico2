# 

## CONFIGURACION:

REQUISITOS:
- memoria SD debe estar formateada en FAT, con MBR principal
- debe haber un archivo llamado "test.txt", con cualquier contenido en texto plano

CONEXIONADO PARA PLACA DE DESARROLLO:
// Pines SPI para la Raspberry Pi Pico 2
#define PIN_MISO  00
#define PIN_CS    01
#define PIN_SCK   02
#define PIN_MOSI  03

MODULO pico-rv32ima, AJUSTES en archivo: $(PROJECT_DIR)/../pico-rv32ima/pico-rv32ima/petitfatfs/mmcbbp.c

#define SD_SPI_INST      spi0
#define SD_SPI_PIN_RX    0   // MISO
#define SD_SPI_PIN_CS    1   // CS
#define SD_SPI_PIN_CK    2   // SCK
#define SD_SPI_PIN_TX    3   // MOSI

### JUN-21-2025

MVP
