# ESPEasy Elektrocas master clock

## Components
 - ESP8266 or ESP32 module, local regulator to 3.3V or addiotional DC/DC buck power supply
 - DC/DC boost power supply set to 24V or 60V(XL6009 module needs output capacitor and diode replaced with 100V rated), optional 200mA PTC on output
 - for 24V or 12V line H bridge like CMOS A4950 or bipolar L298N (higher voltage drop and power consumption)
 - for 60V line 2 relay module (4 relay with separate date line on IPJ0612)
 - 5-12V power supply, 500mA is enough for multiple clocks
 - optional DC/DC UPS module with lithium accumulator, example: https://mysku.ru/blog/taobao/72616.html www.aliexpress.com/item/4000114509953.html

## Software and config
 - ESPEasy https://github.com/letscontrolit/ESPEasy/releases
 - under Tools - Advanced enable NTP and Rules, set correct time zone
 - Rules - paste content of Pragotron_Rules.txt or IBM version, code for date should go to Rules Set 2
 - modify GPIO pins if needed, by default 4 and 5 are used for clock in Pulz event, 12 and 13 for date in Pulz_D event
 - Optional: upload Pragotron.esp to flash, Tools - File browser, it adds simple gui to correct time and manualy adjust for day light saving, access via http://ESP-IP/pragotron.esp


## Diagram
![Diagram](https://raw.github.com/V0JT48/ESPeasyElektrocas/master/ESPEasy.png)
