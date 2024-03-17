# VSCode Settings

That's my personal way of setting up VSCode in terms of formatter >> using prettier, and in terms of linter >> EsLint.

I'm used to using standard rules for my job, so both are set to achieve that purpose. Prettier applies on shortcut formmatting and linter on save shortcut.

## How to use?

Open your vscode settings and click on seeing it as json. Then copy and paste it.

## How to have standard rules working?

In your project, install standard as dev dependency: 

~~~
npm i -D standard
~~~

And then modify your package.json with the following line:

~~~
"eslintConfig": {
    "extends": "./node_modules/standard/eslintrc.json"
}
~~~

*Be aware of erasing any other eslint.config.js file in your path to avoid conflicts*
