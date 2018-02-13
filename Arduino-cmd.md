To program Arduino on Raspberry PI with command line:

- install arduino package

	apt-get install arduino

- stop Octoprint

	/etc/init.d/octoprint stop

- launch avrdude (Arduino version)

	/usr/share/arduino/hardware/tools/avrdude -C /usr/share/arduino/hardware/tools/avrdude.conf -q -q -p m2560 -c wiring -P/dev/ttyUSB0 -D -U flash:w:Marlin.ino.hex:i