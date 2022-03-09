# eslint-prettier-config

run the following commands to install the packeges  
`npm i -D eslint prettier eslint-config-prettier`  
`npm i -D eslint-plugin-import @babel/eslint-parser`  

create `.eslintrc.json` and copy following code and save  
<pre>
{
  "extends": ["eslint:recommended", "plugin:import/errors", "prettier"],
  "rules": {
    "no-console": 1,
    "prefer-const": 2
  },
  "plugins": ["import"],
  "parser": "@babel/eslint-parser",
  "parserOptions": {
    "ecmaVersion": 2019,
    "sourceType": "module",
    "requireConfigFile": false
  },
  "env": {
    "commonjs": true,
    "browser": true,
    "es6": true,
    "node": true
  }
}
</pre>  

create `.prettierrc` and copy following code and save
<pre>
{
    "singleQuote": true
}
</pre>

open `settings.json` and enter the following and save 
<pre>
"editor.defaultFormatter": "esbenp.prettier-vscode",
"prettier.requireConfig": true,
"editor.formatOnSave": true
</pre>
