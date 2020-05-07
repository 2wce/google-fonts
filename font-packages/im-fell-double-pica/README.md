# @expo-google-fonts/im-fell-double-pica

![npm version](https://flat.badgen.net/npm/v/@expo-google-fonts/im-fell-double-pica)
![license](https://flat.badgen.net/github/license/expo/google-fonts)
![publish size](https://flat.badgen.net/packagephobia/install/@expo-google-fonts/im-fell-double-pica)
![publish size](https://flat.badgen.net/packagephobia/publish/@expo-google-fonts/im-fell-double-pica)

This package lets you use the [**IM Fell Double Pica**](https://fonts.google.com/specimen/IM+Fell+Double+Pica) font family from [Google Fonts](https://fonts.google.com/) in your Expo app.

v0.0.3

## IM Fell Double Pica

![IM Fell Double Pica](./font-family.png)

This font family contains [2 styles](#gallery).

- `IMFellDoublePica_Regular400`
- `IMFellDoublePica_Regular400_Italic`

## Usage

Run this command from the shell in the root directory of your Expo project to add the font family package to your project
```sh
expo install @expo-google-fonts/im-fell-double-pica expo-font @use-expo/font
```

Now add code like this to your project
```js
import React, { useState, useEffect } from 'react';

import { Text, View, StyleSheet } from 'react-native';
import { AppLoading } from 'expo';
import { useFonts } from '@use-expo/font';
import {
  IMFellDoublePica_Regular400,
  IMFellDoublePica_Regular400_Italic,
} from '@expo-google-fonts/im-fell-double-pica';

export default () => {
  let [fontsLoaded] = useFonts({
    IMFellDoublePica_Regular400,
    IMFellDoublePica_Regular400_Italic,
  });

  let fontSize = 24;
  let paddingVertical = 6;

  if (!fontsLoaded) {
    return <AppLoading />;
  } else {
    return (
      <View style={{ flex: 1, justifyContent: 'center', alignItems: 'center' }}>
        <Text style={{ fontSize, paddingVertical, fontFamily: 'IMFellDoublePica_Regular400' }}>
          IMFellDoublePica_Regular400
        </Text>

        <Text
          style={{ fontSize, paddingVertical, fontFamily: 'IMFellDoublePica_Regular400_Italic' }}>
          IMFellDoublePica_Regular400_Italic
        </Text>
      </View>
    );
  }
};

```

## 🔡 Gallery

##### IMFellDoublePica_Regular400
![IMFellDoublePica_Regular400](./450b7878b03e1b88b59cd3c88d5a9dab68e698f5e89d49f6bd99bd40514f1eff.ttf.png)

##### IMFellDoublePica_Regular400_Italic
![IMFellDoublePica_Regular400_Italic](./63f80b5f83de7edd9b6a5674a903289d1c0f0679fefe1835d013e2c6910afacd.ttf.png)


## 👩‍💻 Use During Development

If you are trying out lots of different fonts, you can try using the [`@expo-google-fonts/dev` package](https://github.com/expo/google-fonts/tree/master/font-packages/dev#readme).

You can import *any* font style from any Expo Google Fonts package from it. It will load the fonts
over the network at runtime instead of adding the asset as a file to your project, so it may take longer
for your app to get to interactivity at startup, but it is extremely convenient
for playing around with any style that you want.

## 📖 License

The `@expo-google-fonts/im-fell-double-pica` package and its code are released under the MIT license.

All the fonts in the Google Fonts catalog are free and open source.

Check the [IM Fell Double Pica page on Google Fonts](https://fonts.google.com/specimen/IM+Fell+Double+Pica) for the specific license of this font family.

You can use these fonts freely in your products & projects - print or digital, commercial or otherwise. However, you can't sell the fonts on their own. This isn't legal advice, please consider consulting a lawyer and see the full license for all details.

## 🔗 Links

- [IM Fell Double Pica on Google Fonts](https://fonts.google.com/specimen/IM+Fell+Double+Pica)
- [Google Fonts](https://fonts.google.com/)
- [This package on npm](https://www.npmjs.com/package/@expo-google-fonts/im-fell-double-pica)
- [This package on GitHub](https://github.com/expo/google-fonts/tree/master/font-packages/im-fell-double-pica)
- [The Expo Google Fonts project on GitHub](https://github.com/expo/google-fonts)
- [`@expo-google-fonts/dev` Devlopment Package](https://github.com/expo/google-fonts/tree/master/font-packages/dev)


*This file was generated. Instead of editing it by head, please make contributions to [the generator](https://github.com/expo/google-fonts/tree/master/packages/generator)*
