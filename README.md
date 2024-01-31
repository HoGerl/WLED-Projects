# WLED-Projects
WLED Setup for LED Stripes and ESP8266 Controller

# Equipment
- [Diffuser](https://www.amazon.de/dp/B0B17T532Z?&_encoding=UTF8&tag=hogerl-21&linkCode=ur2&linkId=108699c92baa88347f179804e469c9e8&camp=1638&creative=6742)
- [Diffuser for Corner](https://www.amazon.de/-/en/dp/B0BJ7HYSTW?psc=1&amp;ref=ppx_yo2ov_dt_b_product_details&_encoding=UTF8&tag=hogerl0a-21&linkCode=ur2&linkId=328f518b504334cac2e2e492cd7658ab&camp=1638&creative=6742)
- [WS2812B LED Stripe (5m - 30 LEDs/m)](https://www.amazon.de/-/en/dp/B01CDTE9AW?psc=1&amp;ref=ppx_yo2ov_dt_b_product_details&_encoding=UTF8&tag=hogerl0a-21&linkCode=ur2&linkId=a75b4ff38568b7b8e58c7b30cfda0507&camp=1638&creative=6742) - there are more supported, but this gave me the best experience (also tried ws2801)
- [Power Supply - LPV-60](https://www.amazon.de/dp/B00MWQF08C?ref=ppx_yo2ov_dt_b_product_details&amp;th=1&_encoding=UTF8&tag=hogerl0a-21&linkCode=ur2&linkId=1c07d30e5b676f42f0b0a20c126e0014&camp=1638&creative=6742)
- [ESP8266 Controller](https://www.amazon.de/gp/product/B09QRH3KB4/ref=ppx_yo_dt_b_asin_title_o01_s01?ie=UTF8&amp;psc=1&_encoding=UTF8&tag=hogerl0a-21&linkCode=ur2&linkId=c43ca782accbafe8ef0d8d2256297b3b&camp=1638&creative=6742)
- Soldering bit

optional
- Wires for testing
- [Connector Kit](https://www.amazon.de/-/en/gp/product/B0B3DB6Y2X/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&amp;psc=1&_encoding=UTF8&tag=hogerl0a-21&linkCode=ur2&linkId=e43bebb631cf1ae5f0cea00df6e2cf31&camp=1638&creative=6742)
- [DC Connectors](https://www.amazon.de/gp/product/B08RZ38STX/ref=ppx_yo_dt_b_asin_title_o06_s01?ie=UTF8&amp;psc=1&_encoding=UTF8&tag=hogerl0a-21&linkCode=ur2&linkId=d1aeaa60d383fe8e14eaf7debfaa8706&camp=1638&creative=6742)

# software
- [WLED - https://kno.wled.ge/](https://kno.wled.ge/)
- [wled installer (you will need a supported browser, e.g. Chrome) - https://install.wled.me/](https://install.wled.me/)

# starting
the pinout for the esp8266 controller i helpful:

![ESP8266 pinout](https://github.com/HoGerl/WLED-Projects/blob/main/images/ESP8266-NodeMCU-kit-12-E-pinout-gpio-pin.webp)

Basically I work with GPIO 2 / D4 on ESP8266.

## Getting the wired working
the core wiring looks like this:

![wiring](https://github.com/HoGerl/WLED-Projects/blob/main/images/wiring.png)

i am using the DC Connectors for connecting DC to LPV-60 Power supply and LPV-60 power supply to LED Stripe.

Next, connect the ESP Controller to your computer using an usb cable. using a supported browser (e.g. google chrome) to connect via [https://install.wled.me](https://install.wled.me). Select the ESP Controller, install WLED and start configuration after installation. in my cases, i used the gpio 2 port (D4 on ESP Controller).