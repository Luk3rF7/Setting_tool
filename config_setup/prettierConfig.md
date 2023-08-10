<h1 align="center"> Prettier </h1>


<h3>Comandos npm </h3>

<li>npm i -D prettier </li>
<li>npm i -D eslint-config-prettier  </li>
<li>npm i -D eslint-plugin-prettier </li>
<em> Podemos colocar em um linha só </em>

<p>
    arquivo -> .prettierrc.js

        semi -> ;
        trailingComma -> p/ tudo
        singleQuote ->  sempre que possivel
        printWidth ->  largura maxima para quebra linha
        tabWidth -> largura do tab
</p>
<li> config do Prettier:
<p>

      module.exports = {
      arrowParens: 'always',
      bracketSpacing: true,
      endOfLine: 'lf',
      htmlWhitespaceSensitivity: 'ignore',
      insertPragma: false,
      jsxSingleQuote: false,
      printWidth: 80,
      proseWrap: 'always',
      quoteProps: 'as-needed',
      requirePragma: false,
      semi: true,
      singleQuote: true,
      tabWidth: 2,
      trailingComma: 'all',
      useTabs: false,
      vueIndentScriptAndStyle: false,
      embeddedLanguageFormatting: 'off',
      };

</p>
