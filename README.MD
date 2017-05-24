# react-button
> Button component for react.


## properties:
```javascript

  static propTypes = {
    className:PropTypes.string,
    size:PropTypes.oneOf([
      'small',
      'normal',
      'large'
    ]),
    color:PropTypes.string,
    outline:PropTypes.bool,
    round:PropTypes.bool,
    full:PropTypes.bool,
  };

  static defaultProps = {
    size:'normal',
    color:'primary',
    outline:false,
    full:false,
  };
  
```

## usage:
```jsx
class App extends React.Component{
  render(){
    return (
      <div className="hello-react-button" >
        <ReactButton color='primary' size='small'>
          primary button
        </ReactButton>

        <ReactButton color='secondary' size='normal'>
          normal button
        </ReactButton>
        <div className="blank-20"></div>
        <ReactButton full={true} color='wxgreen'>
          normal/wegreen button
        </ReactButton>
        <div className="blank-20"></div>
        <ReactButton color='primary' size='large'>
          primary button
        </ReactButton>
        <div className="blank-20"></div>
        <ReactButton full={true} round={true} color='primary' size='large'>
          primary/full button
        </ReactButton>

        <div className="blank-20"></div>
        <ReactButton color='primary' size='small' outline={true}>
          primary button
        </ReactButton>

        <ReactButton color='secondary' size='normal' outline={true}>
          normal button
        </ReactButton>

    </div>
    );
  }
}

```



## resource:
+ http://ionicframework.com/docs/components/#full-buttons
