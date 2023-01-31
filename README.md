# Phonograph-Pro
[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://github.com/kabouzeid/Phonograph/blob/master/LICENSE.txt)

**A material designed local music player for Android.**

![Screenshots](./art/art.jpg?raw=true)
## Do it yourself
1. Fork the original [Phonograph](https://github.com/kabouzeid/Phonograph) repo
2. Go to `/app/src/main/java/com/kabouzeid/gramophone/App.java`
3. Change the contents of this method: 
```
public static boolean isProVersion() {
    return BuildConfig.DEBUG || 
    app.billingProcessor.isPurchased(PRO_VERSION_PRODUCT_ID);
}
```
&nbsp; &nbsp; &nbsp; &nbsp; To this:
```
public static boolean isProVersion() {
    return true;
}
```
