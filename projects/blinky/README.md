# Der Start: Blinky

Diese Projekt dient nur dazu, die Verbindung zum Raspberry Pi Pico zu testen. Es soll einfach in Thonny
kopiert werden und dann auf den Modul ausgeführt werden, um die Verbindung zwischen der Hardware und der
Entwicklungsumgebung zu testen.

## Der Code

Kopieren Sie folgenden Code in eine neue Datei in Thonny:

```py
from machine import Pin
from time import sleep

pin = Pin(25, Pin.OUT)

while True:
    pin.toggle()
    sleep(1)
```

Drücken Sie in der IDE auf den Play-Button (oder drücken Sie F5), damit das Programm auf dem Pico
ausgeführt wird. Die LED nebem dem USB-Stecker sollte im Sekundenabstand blinken.
