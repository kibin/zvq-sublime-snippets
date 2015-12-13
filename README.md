# zvqsnippets
Snippets for zvooq

### tags
There are several common tags that are expanded in simple tag with tab-triggers
that move your cursor to the positions of className, attributes, content.

These tags are `div`, `span`, `a`, `p`, `ul` and `li`.

There are also two special abstract tags that has another one more tab-trigger.
They are `h` tag which unfolds in `h1` by default with `1` highlighted.
And the `tag` tag which unfolds in `div` by default with `div` highlighted.
The last one is special because you can do any tag with it, just start typing.

##### tag

=>
```javascript
<$1div className=$2$3>$4</$1div>
```

### b_

=>
```javascript
className={this.b_($1)}$2
```

### tyjsx
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

### zjsx
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
