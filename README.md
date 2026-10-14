# ESLint test

If you have bun installed, you can replace npm with bun.

The config in `red/config.toml` sets ESLint as the language server for JavaScript.

1. Run `npm i` to install dependencies
2. Run `npm run dev` to run the project (you can skip it)
3. Run `npm i -g vscode-langservers-extracted@4.8.0` to install `vscode-eslint-language-server` language server
4. Open `src/lib/index.ts` file in Red and you should see `I 'unusedTest' is assigned a value but never used.` if eslint works properly  

Now, what is the problem? People writing frontend pretty much nearly always need both tsserver and eslint language servers at the same time. Right now red allows only a sigle LSP to run at the same time
