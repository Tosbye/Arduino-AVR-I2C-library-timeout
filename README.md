# Arduino AVR I2C library timeout
These two files in this submission implement timeout for I2C operations in AVR architecture. During streaming sensor data from MATLAB it has been observed that AVR based Arduino boards may get stuck in the I2C read or write operation especially if there is a loose connection between the hardware and the I2C device.

# Installation
1. Execute the following command in MATLAB Command Window.
>> fullfile(matlabshared.supportpkg.getSupportPackageRoot, '3P.instrset', 'arduinoide.instrset', 'arduino-1.8.1', 'hardware', 'arduino', 'avr', 'libraries', 'Wire', 'src', 'utility')

This will return a directory. Navigate to that directory.
2. Replaces twi.c and twi.h files with the files shared in this submission.
3. Flash the server on Arduino from MATLAB.
