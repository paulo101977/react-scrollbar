# React Scrollbar

The Simplest Scroll Area Component with custom scrollbar for [React Js](http://facebook.github.io/react/). It's adopted from [reactScrollbar](https://github.com/souhe/reactScrollbar) but without any dependencies. All animation, Height and Width are pure CSS, So it's TOTALLY **CUSTOMIZABLE** and **RESPONSIVE**! YEAH!.

[DEMO](https://bosnaufal.github.io/react-scrollbar)

## Install
You can import [react-scrollbar.js](./src/js/components/react-scrollbar.js) to your react component file like [this](./src/js/components/app.js) and process it with your preprocessor.;



You can install it via NPM
```bash
npm install react-scrollbar-js
```


## Usage
```javascript

import React from 'react';
import ReactDOM from 'react-dom';

import ReactScrollbar from 'react-scrollbar-js';

// Don't Forget to set your webpack configuration file first to handle *.css file
require('react-scrollbar-js/style/react-scrollbar.css')

// Require Your custom styling. ex: .my-scrollbar
require('../../style/my-scrollbar.css')


class App extends React.Component {

  render(){
    return(
      <ReactScrollbar className="my-scrollbar" speed={ 100 } >
        <div className="should-have-a-children scroll-me">
          <p>And Now</p>
          <p>You Can Put</p>
          <p>A Long Content Here</p>
        </div>
      </ReactScrollbar>
    )
  }

}

ReactDOM.render(<App />, document.getElementById("app"))

```


## Props
##### clasess (String)
Just the ordinary class name for styling the wrapper. So, It's TOTALLY **CUSTOMIZABLE!**
```css
/*The Wrapper*/
.my-scrollbar{
  width: 35%;
  min-width: 300px;
  max-height: 450px;
}

/*The Content*/
.scroll-me{
  min-width: 750px;
}
```

##### style (Object)
If you prefer to use inline style to styling the scrollbar, you can pass the styling object to this props.
```javascript
let styling = {

  /* Scrollbar */
  scrollbar: {
    width: "35%",
    minWidth: "300px",
    maxHeight: "450px"
  },

}

<ReactScrollbar style={ styling.scrollbar } />
```

##### speed (Number)
The wheel step in pixel. The default is 53 pixel per wheel.

## Methods
##### scrollToY(y)
To scroll the scrollbar to the Y
```javascript
// Examples
someMethod() {
  this.refs.Scrollbar.scrollToY(100)
}
```

##### scrollToX(x)
To scroll the scrollbar to the X
```javascript
// Examples
someMethod() {
  this.refs.Scrollbar.scrollToX(100)
}
```

## Thank You for Making this useful~

## Let's talk about some projects with me
Just Contact Me At:
- Email: [bosnaufalemail@gmail.com](mailto:bosnaufalemail@gmail.com)
- Skype Id: bosnaufal254
- twitter: [@BosNaufal](https://twitter.com/BosNaufal)

## License
[MIT](http://opensource.org/licenses/MIT)
Copyright (c) 2016 - forever Naufal Rabbani
