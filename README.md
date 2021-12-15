Aura
Phase 1 
• Shall set-up the Raspberry Pi and configure it for the project
o shall instal the Raspbian OS
o shall enamble SPI and I2C I/O
o shall install and setup the SW tools
• Shall demonstrate basic understanding of Python coding 
o Create simple unit conversion program 
• Shall demonstrate basic understanding of Raspberry Pi I/O 
o Configure blue LED on breadboard o Blink LED 
• Shall demonstrate basic understanding of Pygame 
o Add a random rectangle to the center of the game screen 
o Add random ball to the top-left corner of the game screen 
o Add text to the top-right of the game screen

import RPi.GPIO as GPIO
import time
GPIO.setmode(GPIO.BCM)
GPIO.setwarnings(False)
GPIO.setup(19,GPIO.OUT)
for x in range(10):
    time.sleep(1)
    GPIO.output(19,GPIO.HIGH)
    time.sleep(1)
    GPIO.output(19,GPIO.LOW)
