## Installion

```sh
$ yarn global add poi-multi
```

## Usage

```sh
$ poi-multi build index.js
$ poi-multi watch index.js
$ poi-multi dev index.js
```

## Multiple

multiple webpack config supported!

```js
module.export = {
    webpack(config) {
        return [
            config,
            Object.assign({}, config, {
                entry: 'xxx',
                output: {
                    path: 'xxx'
                }
            })
        ]
    }
}
```