# ReactNativeLibrary

## react-redux
```bash
npm install --save react-redux
```

## redux
```bash
npm install --save redux
```

## react-navigation
```bash
npm install --save react-navigation
```

## react-native-tab-view
```bash
npm install react-native-tab-view --save
```

## react-native-vector-icons
### Installation
```bash
npm install react-native-vector-icons --save
react-native link react-native-vector-icons
```
[list icon](https://oblador.github.io/react-native-vector-icons/)

## socket.io-client
```bash
npm install socket.io-client --save
```

## react-native-fbsdk
```bash
react-native install react-native-fbsdk
react-native link react-native-fbsdk
```
[config library](https://github.com/facebook/react-native-fbsdk)

## react-native-facebook-account-kit
```bash
npm install --save react-native-facebook-account-kit
react-native link react-native-facebook-account-kit
```
### For IOS
- Copy `AccountKit.framework` and `AccountKitStrings.bundle` to your project in ios folder
- In xcode, right click -> Add File to "your project" and select 2 files above, remember select the "Copy items if needed" option.
- Add your Facebook credentials to your project's `Info.plist` file
  ```xml
      <plist version="1.0">
        <dict>
          ...
          <key>FacebookAppID</key>
          <string>{your-app-id}</string>
          <key>AccountKitClientToken</key>
          <string>{your-account-kit-client-token}</string>
          <key>CFBundleURLTypes</key>
          <array>
            <dict>
              <key>CFBundleURLSchemes</key>
              <array>
                <string>ak{your-app-id}</string>
              </array>
            </dict>
          </array>
          ...
        </dict>
      </plist>
  ```
### For Android
- In `android/app/src/main/res/values/strings.xml`
   ```xml
   ...
   <string name="fb_app_id">YOUR_FACEBOOK_APP_ID</string>
   <string name="ak_client_token">YOUR_CLIENT_TOKEN</string>
   ```

- In `android/app/src/main/AndroidManifest.xml`
  ```xml
  ...
  <application>

      ...
  
      <meta-data
          android:name="com.facebook.sdk.ApplicationId"
          android:value="@string/fb_app_id" />
      <meta-data
          android:name="com.facebook.accountkit.ApplicationName"
          android:value="@string/app_name" />
      <meta-data
          android:name="com.facebook.accountkit.ClientToken"
          android:value="@string/ak_client_token" />
   </application>
   ...
   ```
   ```js
      //<android:allowBackup="false">
      <android:allowBackup="true">
   ```
- Check the `RNAccountKitPackage` is registered in your `MainApplication.java` file. This should be done by `react-native link` but sometimes it doesn't. You should see something like the following
  ```java
  @Override
  protected List<ReactPackage> getPackages() {
      return Arrays.<ReactPackage>asList(
          new MainReactPackage(),
          new RNAccountKitPackage() // <-- the package is registered
      );
  }
  ```

## react-native-linear-gradient
```bash
npm install react-native-linear-gradient --save
react-native link react-native-linear-gradient
```
## react-native-swiper
```bash
npm install react-native-swiper --save
```

## react-native-fast-image
```bash
npm install react-native-fast-image --save
react-native link react-native-fast-image
```

## react-native-image-picker
```bash
npm install react-native-image-picker@latest --save
react-native link react-native-image-picker
```

## react-native-action-button
```bash
npm i react-native-action-button --save
```

## react-native-circular-action-menu
```bash
npm i react-native-circular-action-menu --save
```

## react-native-textinput-effects
```bash
npm i react-native-textinput-effects --save
```

## react-native-color-picker
```bash
npm install react-native-color-picker --save
```

## react-native-sound
```bash
npm install react-native-sound --save 
react-native link react-native-sound
```

## react-native-splash-screen
[react-native-splash-screen](https://github.com/crazycodeboy/react-native-splash-screen)

## react-native-snap-carousel
[react-native-snap-carousel](https://github.com/archriss/react-native-snap-carousel)

## react-native-maps
[react-native-maps](https://github.com/react-community/react-native-maps)

## react-native-camera
[react-native-camera](https://github.com/react-native-community/react-native-camera)

## react-native-material-design
[react-native-material-design](https://github.com/react-native-material-design/react-native-material-design)
