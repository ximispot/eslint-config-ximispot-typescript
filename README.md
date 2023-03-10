# eslint-config-ximispot-typescript

## This config is used in all internal and external frontend repositories

### The config can be downloaded from NPM

```bash
npm install eslint-config-ximispot-typescript \
            @typescript-eslint/eslint-plugin@latest \
            @typescript-eslint/parser@latest \
            --save-dev
```

### Configure ESLint

If you need Node/Deno support:
```diff
extends: [
+ 'ximispot-typescript/node'
]
```

If you need React support:
```diff
extends: [
+ 'ximispot-typescript/react'
]
```

If you need Vue support:
```diff
extends: [
+ 'ximispot-typescript/vue'
]
```

### Configure the ESLint parser

```diff
{
  extends: ['ximispot-typescript/react'],
+ parserOptions: {
+   project: './tsconfig.json'
+ }
}
```

## License

Open source [licensed as MIT](https://github.com/ximispot/eslint-config-ximispot-typescript/blob/master/LICENSE).