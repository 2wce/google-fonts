# @expo-google-fonts/oxygen

![npm version](https://flat.badgen.net/npm/v/@expo-google-fonts/oxygen)
![license](https://flat.badgen.net/github/license/expo/google-fonts)
![publish size](https://flat.badgen.net/packagephobia/install/@expo-google-fonts/oxygen)
![publish size](https://flat.badgen.net/packagephobia/publish/@expo-google-fonts/oxygen)

This package lets you use the [**Oxygen**](https://fonts.google.com/specimen/Oxygen) font family from [Google Fonts](https://fonts.google.com/) in your Expo app.

v0.0.3

## Oxygen

![Oxygen](./font-family.png)

This font family contains [3 styles](#-gallery).

- `Oxygen_Light300`
- `Oxygen_Regular400`
- `Oxygen_Bold700`

## Usage

Run this command from the shell in the root directory of your Expo project to add the font family package to your project
```sh
expo install @expo-google-fonts/oxygen expo-font
```

Now add code like this to your project
```js
import React, { useState, useEffect } from 'react';

import { Text, View, StyleSheet } from 'react-native';
import { AppLoading } from 'expo';
import {
  Oxygen_Light300,
  Oxygen_Regular400,
  Oxygen_Bold700,
  useFonts,
} from '@expo-google-fonts/oxygen';

export default () => {
  let [fontsLoaded] = useFonts({
    Oxygen_Light300,
    Oxygen_Regular400,
    Oxygen_Bold700,
  });

  let fontSize = 24;
  let paddingVertical = 6;

  if (!fontsLoaded) {
    return <AppLoading />;
  } else {
    return (
      <View style={{ flex: 1, justifyContent: 'center', alignItems: 'center' }}>
        <Text style={{ fontSize, paddingVertical, fontFamily: 'Oxygen_Light300' }}>
          Oxygen_Light300
        </Text>

        <Text style={{ fontSize, paddingVertical, fontFamily: 'Oxygen_Regular400' }}>
          Oxygen_Regular400
        </Text>

        <Text style={{ fontSize, paddingVertical, fontFamily: 'Oxygen_Bold700' }}>
          Oxygen_Bold700
        </Text>
      </View>
    );
  }
};

```

## 🔡 Gallery

##### Oxygen_Light300
![Oxygen_Light300](./a7e1244b4a11ee9f21f86e2f25d7dd963f8e8f93d7b8e411620c959f4cf66fa2.ttf.png)

##### Oxygen_Regular400
![Oxygen_Regular400](./f6497c6c0bb7a884669e84095f3e56550bd7c0ccba79656b0af00d8b3200d790.ttf.png)

##### Oxygen_Bold700
![Oxygen_Bold700](./4bccf594c248e25c3da7e37b9dc5e9cddfcf3bc405504b7d15f4523358d81f76.ttf.png)


## 👩‍💻 Use During Development

If you are trying out lots of different fonts, you can try using the [`@expo-google-fonts/dev` package](https://github.com/expo/google-fonts/tree/master/font-packages/dev#readme).

You can import *any* font style from any Expo Google Fonts package from it. It will load the fonts
over the network at runtime instead of adding the asset as a file to your project, so it may take longer
for your app to get to interactivity at startup, but it is extremely convenient
for playing around with any style that you want.

## 📖 License

The `@expo-google-fonts/oxygen` package and its code are released under the MIT license.

All the fonts in the Google Fonts catalog are free and open source.

Check the [Oxygen page on Google Fonts](https://fonts.google.com/specimen/Oxygen) for the specific license of this font family.

You can use these fonts freely in your products & projects - print or digital, commercial or otherwise. However, you can't sell the fonts on their own. This isn't legal advice, please consider consulting a lawyer and see the full license for all details.

## 🔗 Links

- [Oxygen on Google Fonts](https://fonts.google.com/specimen/Oxygen)
- [Google Fonts](https://fonts.google.com/)
- [This package on npm](https://www.npmjs.com/package/@expo-google-fonts/oxygen)
- [This package on GitHub](https://github.com/expo/google-fonts/tree/master/font-packages/oxygen)
- [The Expo Google Fonts project on GitHub](https://github.com/expo/google-fonts)
- [`@expo-google-fonts/dev` Devlopment Package](https://github.com/expo/google-fonts/tree/master/font-packages/dev)


## 🤝 Contributing

Contributions are very welcome! This entire directory, including what you are reading now, was generated from code. Instead of submitting PRs to this directly, please make contributions to [the generator](https://github.com/expo/google-fonts/tree/master/packages/generator) instead.
