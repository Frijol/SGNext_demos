Demo code for SG_Next presentation
======
August 2016

Accompanying slides are [here](https://docs.google.com/presentation/d/1dVyvq55ieX4W23g0RavFaFcAh9Jvicl1h35ptsOcO6U/edit?usp=sharing)

## Demos

### 01_digital
Demonstration toggling one pin to read on a logic analyzer

### 02_helloSerial
Demonstration of communication over a protocol (serial) to be read on a logic analyzer

### 03_helloAccelerometer
Reads the WHO_AM_I register of accelerometer MMA8452Q over I2C, should return 0x2A over the logic analyzer and print `<Buffer 2a>` to the console

### 04_getZAxis
Reads the OUT_Z_MSB register of accelerometer MMA8452Q over I2C, should print a single hexadecimal value to the console

### 05_pollZAxis
Reads the OUT_Z_MSB register of accelerometer MMA8452Q over I2C at an interval of once per second, should print the same single hexadecimal value to the console over and over (the accelerometer has not been set to "active" mode)

### 06_pollActiveZ
Sets the accelerometer to active mode and then reads the OUT_Z_MSB register of accelerometer MMA8452Q over I2C at an interval of once per second - the value should change as the project is moved

### 07_interpretZ
Reads the changing OUT_Z_MSB register of accelerometer MMA8452Q over I2C at an interval of once per second and interprets/prints to the console whether it is negative or positive

## Tools used
* Microcontroller: [Tessel 2](//tessel.io)
* Part: accelerometer ([Tessel Accelerometer module](//tessel.io/modules))
* Logic analyzer: [Saleae 8](//saleae.com)

## Additional links
* Accelerometer datasheet [MMA8452Q](http://www.nxp.com/files/sensors/doc/data_sheet/MMA8452Q.pdf)
