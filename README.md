# d3-color

> **⚠️ Historical Version Notice**
>
> This is d3-color version 2.x, a historical version maintained for **CommonJS backwards compatibility only**. This version includes security patches but retains CommonJS module support that was removed in version 3.0.0.
>
> **Use this version only if**
>
> - You need CommonJS support (`require()` syntax)
> - You cannot migrate to ES modules (`import`/`export` syntax)
> - You are working with legacy build systems that don't support ES modules
>
> **For new projects, use the latest version** which supports ES modules and receives active development.

## Installing

**For this CommonJS-compatible version**

```bash
npm install @paulchiu/d3-color-common-js
```

**CommonJS usage**

```js
const d3 = require('@paulchiu/d3-color-common-js');
const color = d3.color('steelblue');

// Or with destructuring
const { color, rgb, hsl } = require('@paulchiu/d3-color-common-js');
```

**Using with Legacy Dependencies**

If you have dependencies that require `d3-color` but you need CommonJS support, you can force all packages to use this CommonJS version using package manager overrides:

**With npm (package.json)**

```json
{
  "overrides": {
    "d3-color": "npm:@paulchiu/d3-color-common-js@^2.0.0"
  }
}
```

**With Yarn (package.json)**

```json
{
  "resolutions": {
    "d3-color": "npm:@paulchiu/d3-color-common-js@^2.0.0"
  }
}
```

This will ensure that any package requesting `d3-color` gets this CommonJS-compatible version instead of the official ES module version.

**For the official ES module version**

Please visit <https://d3js.org/d3-color>
