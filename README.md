```const dymensions-frontEnd-guidelines = () => { ```

Below mentioned are the guideliness all the developers in the front-end development team are required to follow to adhere to industry-wide accepted best practices, have a coherent working style, ensure consistency and quality across the codebase and minimize discrepancies.

## Table of Contents

1. [IDE: Visual Studio Code](#ide-visual-studio-code)
2. [Semantic Markup](#semantic-markup)
3. [Naming Convention](#naming-convention)

<h2 id='#ide-visual-studio-code'>IDE: Visual Studio Code</h2>

[VS Code](https://code.visualstudio.com/) is the integrated development environment we use for writing and maintaining our code. You need to install the following extensions which will help you achieve a faster and more productive work style.

<ul>
  <li><a href='https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens'>GitLens - Git supercharged</a></li>
  <li><a href='https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets'>JavaScript (ES6) code snippets</a></li>
  <li><a href='https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode'>Prettier - Code formatter</a></li>
  <li><a href='https://marketplace.visualstudio.com/items?itemName=burkeholland.simple-react-snippets'>Simple React Snippets</a></li>
  <li><a href='https://marketplace.visualstudio.com/items?itemName=shardulm94.trailing-spaces'>Trailing Spaces</a></li>
</ul>

Post installing them, go to vscode settings by pressing <kbd>Ctrl + ,</kbd> and replace the existing ```JSON``` with the following:

```
{
    "editor.wordWrap": "on",
    "files.autoSave": "onFocusChange",
    "explorer.openEditors.visible": 0,
    "editor.formatOnSave": true,
    "prettier.arrowParens": "avoid",
    "prettier.jsxSingleQuote": true,
    "prettier.singleQuote": true,
    "trailing-spaces.trimOnSave": true,
    "window.zoomLevel": 0,
    "[html]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "editor.tabSize": 2,
    "prettier.printWidth": 120,
    "prettier.semi": false,
    "prettier.useEditorConfig": false,
    "[javascript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[javascriptreact]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "emmet.triggerExpansionOnTab": true,
    "emmet.includeLanguages": {
        "javascript": "css"
    },
    "editor.matchBrackets": "never",
    "editor.minimap.enabled": false
}
```

> **Do not** change any of the settings from above except the ```editor fontSize``` in order to maintain a consistent formatting of the code. You are free to install your choice of editor theme and color scheme though.

<h2 id='#semantic-markup'>Semantic Markup</h2>

The generic HTML tags like ```div```, ```span```, ```ul``` etc. are (mostly) used to format content - these tags tell the browser how to display the content on the page. However, they give no indication as to what type of content they contain or what role that content plays in the page.

Semantic HTML5 addresses this shortcoming by defining specific tags. That explicit information helps robots/crawlers like Google and Bing to better understand which content is important, which is a subsidiary, which is for navigation, and so on. By adding semantic HTML tags to your pages, you also add a humman readable structure to the markup like so:

```
<header class='topbar'>
  <h1>Brand Name - Logo</h1>

  <nav>
    <ul>
      <li><a href='#'>Home</a></li>
      <li><a href='#'>About</a></li>
      <li><a href='#'>Contact</a></li>
    </ul>
  </nav>
</header>

<main>
  <section class='services'></section>
</main>

<footer>
  &copy; 2020 All rights reserved
</footer>
```


``` } ```
