# Heat element controller for MSPA Camaro 6P (and others)
Gives the ability to control the heat element of MSPA Tub to adjust heating remote, and to save energy by utilizing periods where energy is cheap .

Hardware:
- NodeMCU ESP32
- Wiring
- DS18B20 waterproof temperatursensor
- 4.7K ohm resistor
- One-channel relay

Configuration:
- Adjust this line to reflect your heat elements size:
          return 1000.0;   # heatelemenet effect in Watt when on
- Adjust this line if you need an offset to the temperatursensor
          offset: 0  # Set your desired temperature offset here

Connect the relay and temperature sensors according to the code (named Dx).
- Relay D14 / GPIO14, GND and 5V/VIN
- Temperaturesensor D4 / GPIO14, GND and 3.3V

I will supply with more pictures later on.

Cut the cable that powers the heater, connect the one phase to relay.
Place the temperaturesensor on the flow pipe and seal it with aluminum tape so get a good temperature reading. Adjust temperaturoffset in code if you need to.
