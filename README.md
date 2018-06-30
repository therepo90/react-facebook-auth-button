# repogames-facebook-auth
Easy to use Facebook auth wrapper

## Usage:

```jsx
import React, { Component } from 'react';
import FacebookAuth from 'repogames-facebook-auth';

class App extends Component {
  state = {
    loggedIn: false,
    fbLoaded: false
  }
  onFBLoad = loggedIn => {
    this.setState({ fbLoaded: true, loggedIn });
  }
  onStatusChange = loggedIn => {
    this.setState({ loggedIn });
  }

  render() {
    return (<FacebookAuth onLoad={this.onFBLoad} appId="Your facebook APP_ID" onStatusChange={this.onStatusChange} />);
  }
}

export default App;
```


