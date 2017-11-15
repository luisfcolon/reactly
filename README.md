# reacli

CLI tool to create react components. Stateless functional or class extended.

__Work in progress__

## Usage

### React class component

```bash
// barebone

reacli make:class ComponentName
```

```javascript
// example output

import React from 'react';


class ComponentName extends React.Component {
  constructor(props) {
    super(props);
  }

  render() {
    return (
      <div className="component" />
    );
  }
}

export default ComponentName;
```

```
// with props

reacli make:class ComponentName -p
```

```javascript
// example output

import React from 'react';

import PropTypes from 'prop-types';


class ComponentName extends React.Component {
  static defaultProps = {};

  static propTypes = {};

  constructor(props) {
    super(props);
  }

  render() {
    return (
      <div className="component" />
    );
  }
}

export default ComponentName;
```

### Stateless functional component

```bash
// barebone

reacli make:functional ComponentName

// with props

reacli make:functional ComponentName -p
```
