# Xiaozhi Sam Board

Hardware summary for the Xiaozhi Sam configuration used by this firmware port.

## Display (ST7789P)

| Function | GPIO | Notes |
|----------|------|-------|
| DC       | GPIO8  | Data/command select |
| CS       | GPIO14 | Chip select |
| SCL      | GPIO9  | SPI clock |
| SDA      | GPIO10 | SPI MOSI |
| RES      | GPIO18 | Display reset |
| BL       | GPIO13 | Backlight PWM |

- Resolution: 284x240 (swap XY, mirror Y)
- Interface: SPI3 @ 80 MHz
- Offsets: X=0, Y=0

## Audio Outputs (Speaker)

| Function | GPIO | Notes |
|----------|------|-------|
| DOUT     | GPIO7  | Speaker data |
| BCLK     | GPIO15 | Bit clock |
| LRCK     | GPIO16 | Left/right clock |

Sample rate: 24 kHz.

## Audio Inputs (Microphone)

| Function | GPIO | Notes |
|----------|------|-------|
| DIN      | GPIO6 | Microphone data |
| SCK      | GPIO5 | Serial clock |
| WS       | GPIO4 | Word select |

Sample rate: 16 kHz.

## Controls

| Function | GPIO | Notes |
|----------|------|-------|
| Boot button | GPIO0  | Boot/OTA trigger |
| Volume +    | GPIO39 | Volume up button |
| Volume -    | GPIO40 | Volume down button |

## Power

| Function | GPIO | Notes |
|----------|------|-------|
| Battery sense | GPIO38 | Battery/charge status |
| Sleep control | GPIO21 | PMU enable (RTC capable) |
