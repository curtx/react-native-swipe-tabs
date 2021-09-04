# react-native-animated-tabs
A simple component that makes tabs animatable.

**Demo**

Works on both IOS and Android.

<img src="https://user-images.githubusercontent.com/89903475/132087155-d333b88d-71b5-4bf3-af84-ecfcc7d477ca.gif" height="500">    <img  src="https://user-images.githubusercontent.com/89903475/132087166-90a98d24-8379-4ba2-b45b-64e57ad1ab64.gif" height="500">

**Installation**

Just run
npm install --save-exact react-native-animated-tabs

**Usage**

Let us suppose there are some screens **"Favourites", "Playlists", "Tracks", "Folders"**

```typescript
import SwipeableTabs from "react-native-animated-tabs"

class Home extends React.Component<any, any>{

    constructor(props: any) {
        super(props)
        this.state = {
            selectedIndex: 0
        }
    }
    
    render() {
        return (
            <SwipeableTabs
                onSwipe={x => this.setState({ selectedIndex: x })}
                selectedIndex={this.state.selection}
            >
                <Favourites />
                <Playlists/>
                <Tracks/>
                <Folders/>
            </SwipeableTabs>)
    }
}
```

**Misc**

Currently I am not allowing pull requests. If you like to suggest a feature, email me to sheharyar.fast@gmail.com. I will get back to you as soon as I can.

