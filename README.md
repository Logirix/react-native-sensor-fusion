# react-native-sensor-fusion with expo-sensors
Version of [react-native-sensor-fusion](https://github.com/cawfree/react-native-sensor-fusion) but with [expo-sensors](https://docs.expo.io/versions/latest/sdk/sensors/)

Documentation is the same as [react-native-sensor-fusion](https://github.com/cawfree/react-native-sensor-fusion))

## Extra methods

With this version of the library you can also use this to know if all the sensors are available for usage:

    import { unsupportedSensors } from 'react-native-sensor-fusion'

    unsupportedSensors().then(function(result) {
      if (result.length === 0) console.log('All required sensors are available')
      else console.log('Missing sensors', result)
    })