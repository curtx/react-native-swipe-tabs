# react-native-swipe-tabs
A simple component that makes tabs animatable.

**Introducing new Version with Labels**

Works on both IOS and Android. Click <a href="https://shahid-sheharyar.web.app/quickdemo" target="_blank" >here</a> to see it in action.

<img  height="500" alt="Screenshot 2022-08-08 at 5 04 21 PM" src="https://user-images.githubusercontent.com/89903475/183413912-2ef538a6-4e42-4cdf-8c1d-6029ce304703.png"> <img src="https://user-images.githubusercontent.com/89903475/132087155-d333b88d-71b5-4bf3-af84-ecfcc7d477ca.gif" height="500">    <img  src="https://user-images.githubusercontent.com/89903475/132087166-90a98d24-8379-4ba2-b45b-64e57ad1ab64.gif" height="500">

**Installation**

Just run
```
npm install --save-exact react-native-swipe-tabs
```
**Update**

Just run 
```
npm install react-native-swipe-tabs@">=1.1.0"
```
**Usage**

Let us suppose there are some screens **"Favourites", "Playlists", "Tracks", "Folders"**

Pass **labels** prop like below to display TabBar

```tsx
import SwipeableTabs from "react-native-swipe-tabs"
....
class Home extends React.Component<any, any>{

    constructor(props: any) {
        super(props)
        this.state = {
            selectedIndex: 0
        }
    }
    
    render() {
     return (<SwipeableTabs
                onSwipe={x => this.setState({ selectedIndex: x })}
                selectedIndex={this.state.selectedIndex}
                labels={["Favourites","Playlists","Tracks","Folders"]}
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

