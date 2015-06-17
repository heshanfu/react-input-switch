# react-input-switch
Switch component
### Installation
``` sh
npm install react-input-switch --save
```
### Usage
``` javascript
var App = React.createClass({
  getInitialState() {
    return {
      checked: false
    };
  },

  render() {
    return (
      <div>
        <InputSwitch
          checked={this.state.checked}
          onChange={this.handleChange}
        />
        <div>{this.state.checked ? 'checked' : 'unchecked'}</div>
      </div>
    );
  },

  handleChange(checked) {
    this.setState({
      checked: checked
    });
  }
});

```
