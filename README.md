# ESLint Config

Very minimal eslint config for JavaScript and TypeScript Node projects.

## Usage

Just install and use as thus:

### JavaScript

Intall the package as a dev dependency:

```sh
yarn add --dev @akhilome/eslint-config
```

Create an ESLint config file in the root of your project:

```sh
echo 'extends: "@akhilome/eslint-config"' > .eslintrc.yml
```

> Ensure the package's required peer dependencies - `eslint >= 8.0.0`, `prettier >= 2.0.0` are installed.

### TypeScript

Intall the package as a dev dependency:

```sh
yarn add --dev @akhilome/eslint-config
```

Create an ESLint config file in the root of your project:

```sh
echo 'extends: "@akhilome/eslint-config/ts"' > .eslintrc.yml
```

Create [if not exists] a `tsconfig.eslint.json` file with the following content:

```json
{
  "extends": "./tsconfig.json",
  "include": ["./*.ts", "src", "test", "tests"],
  "exclude": [""]
}
```

> Ensure the package's required peer dependencies - `eslint >= 8.0.0`, `prettier >= 2.0.0`, `typescript >= 4.0.0` are installed.
