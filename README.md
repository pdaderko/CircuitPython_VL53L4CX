CircuitPython library for VL53L4CX

Slightly modified version of Adafruit's VL53L1X library ( https://github.com/adafruit/Adafruit_CircuitPython_VL53L1X/ ) with a little bit from the VL53L4CD library ( https://github.com/adafruit/Adafruit_CircuitPython_VL53L4CD/ ) to support the VL53L4CX.

The sensor is supposed to support up to 6m range, though I'm generally seeing just over 4m max range, so the settings may not be perfect.  The VL53L1X supports up to 4m range, and this code uses the VL53L1X settings, so that may be the reason.

In my testing, ST's Arduino code ( https://github.com/stm32duino/VL53L4CX ) was also maxing out around 4m, so I'm not sure whether my test environment is affecting the range, or if their code isn't optimal either.

This was tested on the ESP32-S3 Reverse TFT Feather.
