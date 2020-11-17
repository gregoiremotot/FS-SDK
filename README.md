# Game React Native Feeling Sports SDK
## Install the SDK
```
npm install PRIVATE_REPO/game-react-native-feeling-sports-sdk
```

## Usage

### Mini Game

```js
import React, { Component } from 'react';
import { View } from 'react-native';
import { MiniGameFeelingSports } from 'game-react-native-feeling-sports-sdk';

export default class MiniGame extends Component {
  render() {
    return (
      <View>
        <MiniGameFeelingSports
          gameId=["Unique game id like : 'homepage-{id}' or 'matchcenter-{id}'"]
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
      </View>
    );
  }
};
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
          gameId=["Unique game id like : 'homepage-{id}' or 'matchcenter-{id}'"]
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
