# My settings of VSCode, ESLint.

I will be updating this in future as per my needs.

## Enable JSX support for React Development in VSCode.

- Add below written setting to your **workspace setting** in which your react project is located.

  ```json
  "files.associations": {
    "*.js": "javascriptreact"
  }
  ```

  or add this to **user settings**

  ```json
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  },
  ```

## Integrate ESLint with Prettier (For JS Projects)

- Install the ESLint & Prettier extension for VSCode. (Keep prettier for other languages also. I will be using prettier as node_module.)

- Open the **VSCode** settings file and add these rules.

  ```json
  "editor.formatOnSave": true,
  "[javascript]": {
    "editor.formatOnSave": false
  },
  // eslint settings
  "eslint.autoFixOnSave": true,
  "eslint.alwaysShowStatus": true,
  ```

- Install `eslint` module as **dev-dependency** using npm and setup a `.eslintrc` file.

- Install `prettier`, `eslint-plugin-prettier` & `eslint-config-prettier` using npm.

- Copy my `.eslintrc` file & change the eslint rules accordig to your choice.
