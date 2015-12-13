# zvqsnippets
Snippets for zvooq

### b_

=>
```javascript
className={this.b_($1)}$2
```

### createcomponent
(for TY)
=>
```javascript
require('./<$1filename>.styl');

const
  <$2filename> = React.createClass({
    mixins: [ Bem ],
    render() {
      return (
        <div className={this.b_()}>
          <div className={this.b_('-content')}>
            $3
          </div>
        </div>
      );
    }
  });
  
module.exports = <$2filename>;
```

### zvooqcomponent 
(for ZVOOQ)
=>

```javascript
goog.provide('zvq.components.<$1filename>');

goog.require('zvq.components.mixins.BEM');

zvq.components.<$1filename> = React.createClass({
  mixins: [ zvq.components.mixins.BEM ],
  render() {
    return (
      $2
    );
  }
});
```
