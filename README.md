
# react-native-bluetooth-classic-hex

React Native Bluetooth Classic Hex is basically to provide the HEX data communtication. 

Based off the [react-native-bluetooth-classic](https://github.com/kenjdavidson/react-native-bluetooth-classic), and updated to support the Hexadecimal data communication.

## Read data
```
 const data = await RNBluetoothClassic.readFromDevice(); 
```

## Write data
```
npm install buffer

const Buffer = require('buffer/').Buffer;

writeData = async (data) => {
    const dataToWrite = new Buffer.from(data, 'hex');
    await RNBluetoothClassic.write(dataToWrite);
  };
```
