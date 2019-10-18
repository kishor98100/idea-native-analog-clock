# React Native: react-native-clock-analog

[![GitHub package version](https://img.shields.io/github/package-json/v/kishor98100/idea-native-analog-clock)](https://github.com/kishor98100/idea-native-analog-clock)
[![github home](https://img.shields.io/npm/v/idea-native-clock)](https://www.npmjs.com/package/idea-native-clock)
![platforms](https://img.shields.io/badge/platforms-Android%20%7C%20iOS-brightgreen.svg?style=flat&colorB=191A17)
[![github home](https://img.shields.io/badge/kishor98100-idea--native--clock-blue)](https://github.com/kishor98100/idea-native-analog-clock)


[![github license](https://img.shields.io/npm/l/idea-native-clock)](https://github.com/kishor98100/idea-native-analog-clock)

<!-- <img src="https://github.com/gaetanozappi/react-native-clock-analog/raw/master/screenshot/react-native-clock-analog.png" /> -->

-   [Usage](#-usage)
-   [License](#-license)

## 📖 Getting started

`$ npm install idea-native-clock --save`


## 💻 Usage

```javascript
import * as React from 'react';
import { StyleSheet, Text, View, ImageBackground } from 'react-native';

import AnalogClock from 'idea-native-clock';

export default class App extends React.Component {
  render() {
    return (
      <View style={styles.container}>
       
       //automatic time
          <AnalogClock
            size={100}
          />
          <View style={{ marginBottom: 5 }} />

          //if you want to set time manually 
          <AnalogClock
            colorClock="#2196F3"
            colorNumber="#000000"
            colorCenter="#00BCD4"
            colorHour="#FF8F00"
            colorMinutes="#FFC400"
            hour="2"
            minutes={55}
            seconds={60}
          />
      </View>
    );
  }
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    alignItems: 'center',
    justifyContent: 'center',
    backgroundColor: '#ecf0f1',
    padding: 8,
  },
});
```

## 💡 Props

| Prop              | Type       | Default | Note                                                                                                       |
| ----------------- | ---------- | ------- | ---------------------------------------------------------------------------------------------------------- |
| `size`       | `number`   |  `180`  | Clock size.
| `colorClock`      | `string`   | `rgba(255,255,255,0.8)` | Clock color.
| `colorNumber`      | `string`   | ![#ffffff](https://placehold.it/15/ffffff/000000?text=+) `#ffffff` | Color of the clock numbers.
| `colorCenter`      | `string`   | ![#ffffff](https://placehold.it/15/ffffff/000000?text=+) `#ffffff` | Clock center color.
| `colorHour`      | `string`   | ![#ffffff](https://placehold.it/15/ffffff/000000?text=+) `#ffffff`  | Clock hour hand color.
| `colorMinutes`      | `string`   | `rgba(255,255,255,0.7)`  | Clock minute  hand color.
| `colorSeconds`      | `string`   | `rgba(255,255,255,0.7)`  | Clock  Second hand color.
| `hour`      | `number`   |  | Hour.
| `minutes`      | `number`   |  | Minutes.
| `seconds`      | `number`   |  | Seconds.

## 📜 License
This library is provided under the MIT License.
