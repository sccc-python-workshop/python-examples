# Sample Code for SCCC Python + Arduino Workshop


# Setting up ardunio

You need to download the arduino software from:

https://www.arduino.cc/en/Main/Donate

There are versions for Windows, Linux, and Mac.

Once you install it, take a note of where it finds your arduino board
(under Tools/Port).  On Windows this will be something like "COM4" on
Linux it will be something like "/dev/ttyUSB0"

## Linux permissions

You installed the software as a user, so you need to make sure that
you have permissions to write to the USB port.  This can be
acccomplished as root by

```
chmod a+rw /dev/ttyUSB0 
```

## Loading Standard Firmata

To communicate with the board using python, you need to install the
`pyfirmata` package.  This can be done via your package manager or
`pip`, e.g., as

```
pip install pyfirmata
```

In the arduino application, do "File/Examples/Firmata/StandardFirmata"
and upload it (using the -> icon) to your device.  If it is successful,
you are ready to play.


