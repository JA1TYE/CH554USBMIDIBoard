# CH554 USB-MIDI Host Board

This board is designed to use [WCH's 8-bit MCU CH554](http://wch-ic.com/products/CH554.html) as a USB-MIDI Host.

Firmware for this board is available on [CH554USBMIDIHost](https://github.com/JA1TYE/CH554USBMIDIHost).

## How to use
CH554's UART0(TX:P3.1/RX:P3.0) are used as MIDI 1.0 I/F. 
CH554's UART1(TX:P1.7/RX:P1.6) are used for debugging.

This board have MIDI 1.0 compatible TX circuit(some resistors to consist current loop) but circuit for RX(i.e. optoisolator) is not contained. If you use MIDI1.0 RX, you should add optoisolator and so on.

You can use USB-A port and DEBUG UART (UART1) port to write firmware to CH554.
You need to power on with pressing SW1 to enter bootloader mode.