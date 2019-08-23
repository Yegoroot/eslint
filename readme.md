## Step 1

- Install eslint plugin for vscode
- Install eslint (you can also install this globally but I like to install it locally)

```
yarn add eslint -D
```

- Install eslint-config-airbnb which need few other dependencies as well

```
yarn add eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react -D
```

- Create .eslintrc file in the root directory and add the following lines

## Step 2

- Install prettier and related dependencies

```
yarn add prettier eslint-config-prettier eslint-plugin-prettier -D
```

- Update .eslintrc with following lines
  looking for **.eslintrc**

## Step 3

```json
{
  // other settings
  // formatting using eslint
  // let editor format using prettier for all other files
  "editor.formatOnSave": true,
  // disable editor formatting, so eslint can handle it
  "[javascript]": {
    "editor.formatOnSave": false
  },
  // available through eslint plugin in vscode
  "eslint.autoFixOnSave": true,
  "eslint.alwaysShowStatus": true
}
```
