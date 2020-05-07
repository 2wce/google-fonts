# @expo-google-fonts/quattrocento-sans

![npm version](https://flat.badgen.net/npm/v/@expo-google-fonts/quattrocento-sans)
![license](https://flat.badgen.net/github/license/expo/google-fonts)
![publish size](https://flat.badgen.net/packagephobia/install/@expo-google-fonts/quattrocento-sans)
![publish size](https://flat.badgen.net/packagephobia/publish/@expo-google-fonts/quattrocento-sans)

This package lets you use the [**Quattrocento Sans**](https://fonts.google.com/specimen/Quattrocento+Sans) font family from [Google Fonts](https://fonts.google.com/) in your Expo app.

v0.0.3

## Quattrocento Sans

![Quattrocento Sans](./font-family.png)

This font family contains [4 styles](#gallery).

- `QuattrocentoSans_Regular400`
- `QuattrocentoSans_Regular400_Italic`
- `QuattrocentoSans_Bold700`
- `QuattrocentoSans_Bold700_Italic`

## 🔡 Usage

Run this command from the shell in the root directory of your Expo project to add the font family package to your project
```sh
expo install @expo-google-fonts/quattrocento-sans expo-font @use-expo/font
```

Now add code like this to your project
```js
import React, { useState, useEffect } from 'react';

import { Text, View, StyleSheet } from 'react-native';
import { AppLoading } from 'expo';
import { useFonts } from '@use-expo/font';
import {
  QuattrocentoSans_Regular400,
  QuattrocentoSans_Regular400_Italic,
  QuattrocentoSans_Bold700,
  QuattrocentoSans_Bold700_Italic,
} from '@expo-google-fonts/quattrocento-sans';

export default () => {
  let [fontsLoaded] = useFonts({
    QuattrocentoSans_Regular400,
    QuattrocentoSans_Regular400_Italic,
    QuattrocentoSans_Bold700,
    QuattrocentoSans_Bold700_Italic,
  });

  let fontSize = 24;
  let paddingVertical = 6;

  if (!fontsLoaded) {
    return <AppLoading />;
  } else {
    return (
      <View style={{ flex: 1, justifyContent: 'center', alignItems: 'center' }}>
        <Text style={{ fontSize, paddingVertical, fontFamily: 'QuattrocentoSans_Regular400' }}>
          QuattrocentoSans_Regular400
        </Text>

        <Text
          style={{ fontSize, paddingVertical, fontFamily: 'QuattrocentoSans_Regular400_Italic' }}>
          QuattrocentoSans_Regular400_Italic
        </Text>

        <Text style={{ fontSize, paddingVertical, fontFamily: 'QuattrocentoSans_Bold700' }}>
          QuattrocentoSans_Bold700
        </Text>

        <Text style={{ fontSize, paddingVertical, fontFamily: 'QuattrocentoSans_Bold700_Italic' }}>
          QuattrocentoSans_Bold700_Italic
        </Text>
      </View>
    );
  }
};

```

## 📖 Gallery

##### QuattrocentoSans_Regular400
![QuattrocentoSans_Regular400](./114280821a2f8698d737c5c9bcbc986cf36a4dbd9fa7c58e448b35520a6053ec.ttf.png)

##### QuattrocentoSans_Regular400_Italic
![QuattrocentoSans_Regular400_Italic](./c933f0ba971f5573109a7674a40f980252c7f3c810a75f9ff29c016102118e85.ttf.png)

##### QuattrocentoSans_Bold700
![QuattrocentoSans_Bold700](./1a542b5aa650f5ce3fa5e6b692feef037c10962d8ae63545c47fdf964e5b3e26.ttf.png)

##### QuattrocentoSans_Bold700_Italic
![QuattrocentoSans_Bold700_Italic](./edadcb4799c44215ae17124bc3eac621aef5a4348743df4d74ff83fd09a601a4.ttf.png)


## 🖥️ Use During Development

If you are trying out lots of different fonts, you can try using the [`@expo-google-fonts/dev` package](https://github.com/expo/google-fonts/tree/master/font-packages/dev#readme).

You can import *any* font style from any Expo Google Fonts package from it. It will load the fonts
over the network at runtime instead of adding the asset as a file to your project, so it may take longer
for your app to get to interactivity at startup, but it is extremely convenient
for playing around with any style that you want.

## ⚖️ License

The `@expo-google-fonts/quattrocento-sans` package and its code are released under the MIT license.

All the fonts in the Google Fonts catalog are free and open source.

Check the [Quattrocento Sans page on Google Fonts](https://fonts.google.com/specimen/Quattrocento+Sans) for the specific license of this font family.

You can use these fonts freely in your products & projects - print or digital, commercial or otherwise. However, you can't sell the fonts on their own. This isn't legal advice, please consider consulting a lawyer and see the full license for all details.

## 🔗 Links

- [Quattrocento Sans on Google Fonts](https://fonts.google.com/specimen/Quattrocento+Sans)
- [Google Fonts](https://fonts.google.com/)
- [This package on npm](https://www.npmjs.com/package/@expo-google-fonts/quattrocento-sans)
- [This package on GitHub](https://github.com/expo/google-fonts/tree/master/font-packages/quattrocento-sans)
- [The Expo Google Fonts project on GitHub](https://github.com/expo/google-fonts)
- [`@expo-google-fonts/dev` Devlopment Package](https://github.com/expo/google-fonts/tree/master/font-packages/dev)


*This file was generated. Instead of editing it by head, please make contributions to [the generator](https://github.com/expo/google-fonts/tree/master/packages/generator)*
