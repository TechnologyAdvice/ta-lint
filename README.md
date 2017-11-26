# ta-lint

All-in-one linting utilities.

## Installation

```sh
yarn add --dev ta-lint
```

### Prettier

Create a `prettier.config.json` in the root of your project that exports our standard configuration:

```js
// prettier.config.js
module.exports = require('ta-lint/configs/prettier')
```

That's all you need to run prettier in your project! If you'd like, you can setup convenient npm scripts in your `package.json`:

```json
{
  "scripts": {
    "prettier": "prettier \"{src,tests}/**/*.{js,ts,tsx}\"",
    "prettier:fix": "npm run prettier -- --write"
  }
}
```
