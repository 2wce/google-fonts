# @expo-google-fonts/caveat

![npm version](https://flat.badgen.net/npm/v/@expo-google-fonts/caveat)
![license](https://flat.badgen.net/github/license/expo/google-fonts)
![publish size](https://flat.badgen.net/packagephobia/install/@expo-google-fonts/caveat)
![publish size](https://flat.badgen.net/packagephobia/publish/@expo-google-fonts/caveat)

This package lets you use the [**Caveat**](https://fonts.google.com/specimen/Caveat) font family from [Google Fonts](https://fonts.google.com/) in your Expo app.

v0.0.3

## Caveat

![Caveat](./font-family.png)

This font family contains [2 styles](#-gallery).

- `Caveat_Regular400`
- `Caveat_Bold700`

## Usage

Run this command from the shell in the root directory of your Expo project to add the font family package to your project
```sh
expo install @expo-google-fonts/caveat expo-font @use-expo/font
```

Now add code like this to your project
```js
import React, { useState, useEffect } from 'react';

import { Text, View, StyleSheet } from 'react-native';
import { AppLoading } from 'expo';
import { useFonts } from '@use-expo/font';
import { Caveat_Regular400, Caveat_Bold700 } from '@expo-google-fonts/caveat';

export default () => {
  let [fontsLoaded] = useFonts({
    Caveat_Regular400,
    Caveat_Bold700,
  });

  let fontSize = 24;
  let paddingVertical = 6;

  if (!fontsLoaded) {
    return <AppLoading />;
  } else {
    return (
      <View style={{ flex: 1, justifyContent: 'center', alignItems: 'center' }}>
        <Text style={{ fontSize, paddingVertical, fontFamily: 'Caveat_Regular400' }}>
          Caveat_Regular400
        </Text>

        <Text style={{ fontSize, paddingVertical, fontFamily: 'Caveat_Bold700' }}>
          Caveat_Bold700
        </Text>
      </View>
    );
  }
};

```

## 🔡 Gallery

##### Caveat_Regular400
![Caveat_Regular400](./0ffe3acdd9c8d91838d7ba021d1c4e9111151e34a104318a8aafe0efeda5755f.ttf.png)

##### Caveat_Bold700
![Caveat_Bold700](./6993da01fa90c359d45a03be9927b46be80d261978de6f5805f43d75ed2d172f.ttf.png)


## 👩‍💻 Use During Development

If you are trying out lots of different fonts, you can try using the [`@expo-google-fonts/dev` package](https://github.com/expo/google-fonts/tree/master/font-packages/dev#readme).

You can import *any* font style from any Expo Google Fonts package from it. It will load the fonts
over the network at runtime instead of adding the asset as a file to your project, so it may take longer
for your app to get to interactivity at startup, but it is extremely convenient
for playing around with any style that you want.

## 📖 License

The `@expo-google-fonts/caveat` package and its code are released under the MIT license.

All the fonts in the Google Fonts catalog are free and open source.

Check the [Caveat page on Google Fonts](https://fonts.google.com/specimen/Caveat) for the specific license of this font family.

You can use these fonts freely in your products & projects - print or digital, commercial or otherwise. However, you can't sell the fonts on their own. This isn't legal advice, please consider consulting a lawyer and see the full license for all details.

## 🔗 Links

- [Caveat on Google Fonts](https://fonts.google.com/specimen/Caveat)
- [Google Fonts](https://fonts.google.com/)
- [This package on npm](https://www.npmjs.com/package/@expo-google-fonts/caveat)
- [This package on GitHub](https://github.com/expo/google-fonts/tree/master/font-packages/caveat)
- [The Expo Google Fonts project on GitHub](https://github.com/expo/google-fonts)
- [`@expo-google-fonts/dev` Devlopment Package](https://github.com/expo/google-fonts/tree/master/font-packages/dev)


*This entire directory, including this README, was generated from code. Instead of submitting PRs to this directly, please make contributions to [the generator](https://github.com/expo/google-fonts/tree/master/packages/generator)*
