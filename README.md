# oak-tree <!-- omit in toc -->
Oak tree, a GIVE Tree implementation with variable interval, no summary, auto-balanced (B+ tree) properties.

- [Install](#install)
- [Usage](#usage)

# Install
```bash
npm install @givengine/oak-tree
```

# Usage
You may import the entire namespace of `OakTree`, which includes `OakTree`, and `OakNode`:
```javascript
// Import namespace
const OakTreeNS = require('@givengine/oak-tree')

// Instantiate an Oak tree
var myOakTree = new OakTreeNS.OakTree('chr1:1-100000000')

// Extend your own tree and/or nodes
class MySpecialOakTree extends OakTreeNS.OakTree {
  // Extension code here
}

class MySpecialOakNode extends OakTreeNS.OakNode {
  // Extension code here
}
```

Or you may selectively import part of the module (if you only want to use `OakTree` this may be a better way):
```javascript
// Import tree definition only
const OakTree = require('@givengine/oak-tree').OakTree

// Instantiate an Oak tree
var myOakTree = new OakTree('chr1:1-100000000')
```
