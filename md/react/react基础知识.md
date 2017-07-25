 <h1>React基础知识详解</h1>
<p style="color:#777">除组件化、虚拟DOM在复用以及性能上带来的一般好处外，React思想使得开发者之间更好的分工与合作，在配合上非常顺畅，规范的接口以及极强的约束，使得整个代码结构清晰，不同开发者的代码高度一致。</p>
<h2>1.顶层API</h2>
<p>最简单的React组件及其渲染</p>
```js
import React, { Component } from 'react';

/**
 * 最简单的一个组件
 */
class SimpleComponent extends Component {
  render(){
    return <div> here we go </div>;
  }
}

// 我们可以看看React给我们提供了哪些顶层组件
console.log( React );

export default SimpleComponent;
```
<h3>react.js</h3>
```js
React.Children: Object
React.Component: ReactComponent(props, context, updater)
React.DOM: Object
React.PropTypes: Object
React.cloneElement: (element, props, children)
React.createClass: (spec)
React.createElement: (type, props, children)
React.createFactory: (type)
React.createMixin: (mixin)
React.isValidElement: (object)
```
<span>Component API</span>
```js
this.context: Object
this.props: Object
this.refs: Object
this.state: Object
this.setState: Object
```
### react-dom.js
```js
ReactDOM.findDOMNode: findDOMNode(componentOrElement)
ReactDOM.render: ()
ReactDOM.unmountComponentAtNode: (container)
```
### react-dom-server.js
```js
ReactDOMServer.renderToString
ReactDOMServer.renderToStaticMarkup
```
## 2. jsx语法

<span>类似 xml 的语法，用来描述组件树</span>
