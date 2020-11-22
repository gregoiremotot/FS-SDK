# Game React Native Feeling Sports SDK
## Install the SDK
```
npm install PRIVATE_REPO/game-react-native-feeling-sports-sdk
```

## Usage

### Mini Game

```js
<MiniGameFeelingSports
  userId={""} // user id if the user is connected
  gameId={""} // Unique game id like : 'homepage-{id}' or 'matchcenter-{id}'
  onCallToActionCliked={
    (error, result) => {
      switch (result) {
        case 'PAGE_REDIRECT_GAMING_ZONE':
          // redirect the user to the Gaming Zone page
          break;
         // ...
       }
     }
  }
/>
```

### Full Game

```js
import React, { Component } from 'react';
import { View } from 'react-native';
import { FullGameFeelingSports } from 'game-react-native-feeling-sports-sdk';

export default class FullGame extends Component {
  render() {
    return (
      <View>
        <FullGameFeelingSports
          userId={""} // user id if the user is connected
          onCallToActionCliked={
            (error, result) => {
              switch (result) {
                case 'PAGE_REDIRECT_MATCH_CENTER':
                  // redirect the user to the Match Center page
                  break;
                 // ...
               }
             }
           }
        />
      </View>
    );
  }
};
```


### Profile Gaming

```js
<ProfileGamingFeelingSports
  userId={""} // user id if the user is connected
/>
```

### Edition Plugin

```js
<!-- Feeling Sports Edition Plugin -->
<div id=''></div>
<script async src='PRIVATE_REPO/edition-plugin.js?clientId=FS-XX'></script>
<!-- End Feeling Sports Edition Plugin -->
```

