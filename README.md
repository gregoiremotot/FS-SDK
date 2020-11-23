# Game React Native Feeling Sports SDK
## Install the SDK
```
npm install PRIVATE_REPO/game-react-native-feeling-sports-sdk
```

## Usage

### Mini Game

```js
<FSMiniGame
  authToken={""} // Optional, if the user is connected
  gameId={""} // Unique game id like : 'homepage-{id}', 'matchcenter-{id}' or 'ondemand-{id}'
  onCallToActionCliked={
    (error, result) => {
      switch (result) {
        case 'PAGE_REDIRECT_GAMING_ZONE':
          // Redirect the user to the Gaming Zone page
          break;
        // ...
      }
    }
  }
/>
```

### Full Game

```js
<FSFullGame
  authToken={""} // Optional, if the user is connected
  onCallToActionCliked={
    (error, result) => {
      switch (result) {
        case 'PAGE_REDIRECT_MATCH_CENTER':
          // Redirect the user to the Match Center page
          break;
        // ...
      }
    }
  }
/>
```


### Profile Gaming

```js
<FSProfileGaming
  authToken={""} // Optional, if the user is connected
  onCallToActionCliked={
    (error, result) => {
      switch (result) {
        case 'PAGE_REDIRECT_GAMING_ZONE':
          // Redirect the user to the Gaming Zone page
          break;
        // ...
      }
    }
  }
/>
```

### Edition Plugin

```js
<!-- Feeling Sports Edition Plugin -->
<div id='fs-edition-plugin'></div>
<script async src='PRIVATE_REPO/edition-plugin.js?clientId=FS-XX'></script>
<!-- End Feeling Sports Edition Plugin -->
```

