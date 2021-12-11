# ESPEasy Elektrocas master clock

## Components
 - ESP8266 or ESP32 module, local regulator to 3.3V or addiotional DC/DC buck power supply
 - DC/DC boost power supply set to 24V or 60V(XL6009 module needs output capacitor and diode replaced with 100V rated), optional 200mA PTC on output
 - for 24V or 12V line H bridge like CMOS A4950 or bipolar L298N (higher voltage drop and power consumption)
 - for 60V line 2 relay module (4 relay with separate date line on IPJ0612)
 - 5-12V power supply, 500mA is enough for multiple clocks
 - optional DC/DC UPS module with lithium accumulator, example: https://mysku.ru/blog/taobao/72616.html www.aliexpress.com/item/4000114509953.html

## Diagram
![Diagram](https://raw.github.com/V0JT48/ESPeasyElektrocas/master/ESPEasy.png)
