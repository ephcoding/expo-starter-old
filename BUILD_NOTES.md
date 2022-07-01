# APP STARTERS

- amazon-archives/[aws-mobile-react-native-starter](https://github.com/amazon-archives/aws-mobile-react-native-starter)
- flatlogic/[react-native-starter](https://github.com/flatlogic/react-native-starter)
- infinitered/[ignite](https://github.com/infinitered/ignite)
- mcnamee/[react-native-expo-starter-kit](https://github.com/mcnamee/react-native-expo-starter-kit)

# BACKEND

- amazon-archives/[aws-mobile-react-native-starter](https://github.com/amazon-archives/aws-mobile-react-native-starter/tree/master/backend)
- [GraphQL crash course](https://www.youtube.com/watch?v=BcLNfwF04Kw)

# COMPONENTS / DESIGN SYSTEM / UI

- flatlogic/[react-native-starter/src/styles](https://github.com/flatlogic/react-native-starter/tree/master/src/styles)
- Shopify/[polaris](https://github.com/Shopify/polaris)
- theme/ files from [@expo/styleguide-native](https://github.com/expo/styleguide/tree/main/packages/styleguide-native/src/styles)

# GLOBAL INSTALLS

- [react-native-debugger](https://github.com/jhen0409/react-native-debugger#documentation)

# TESTING

- type checking with [Flow](https://flow.org/en/docs/install/)

# TOOLING

## Modify App Entry Point (ie. move App.js to app/App.js)

- Expo [app entry point](https://docs.expo.dev/build-reference/migrating/#custom--main--entry-point-in)

  ```json
  <!-- remove from package.json -->
  "main": "node_modules/expo/AppEntry.js"

  <!-- create and add to <root>/index.js -->
  import { registerRootComponent } from 'expo';
  import App from './src/App';
  ```

registerRootComponent(App);
