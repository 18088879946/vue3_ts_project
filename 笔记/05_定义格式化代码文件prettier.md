#### 简介

```javas
eslint是检查代码语法错误，
prettier配置是配置关于格式化代码（这个也可以在vscode中的settting.json文件中配置）
```

#### setting.json文件的配置

```json
{
  "open-in-browser.default": "chrome",
  "editor.formatOnSave": true,
  "liveServer.settings.donotShowInfoMsg": true,
  "px2vw.width": 375,
  "previewServer.browsers": ["chrome"],
  "window.commandCenter": false,
  "vetur.ignoreProjectWarning": true,
  //保存到额时候用使用prettier进行格式化

  // 默认使用prittier作为格式化工具
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "explorer.compactFolders": false,
  "editor.minimap.enabled": false,
  "cssrem.rootFontSize": 75,
  "auto-rename-tag.activationOnLanguage": ["*"]

  // 不要有分号
  // "prettier.semi": false,

  // // 使用单引号
  // "prettier.singleQuote": true,

  // "prettier.trailingComma": "none"
}

```

#### 也可以在下载插件配置格式化

```javas
npm install -D eslint-plugin-prettier prettier eslint-config-prettier
```

#### prettierrc.json添加规则

```javas
{
	"singleQuote":true,
	"semi":false,
	"bracketSpacing":true,
	"htmlWhitespaceSensitivity":"ignore",
	"endOfLine":"auto",
	"trailingComma":"all",
	"tabWidth":2
}
```

#### prettierignore忽略文件

```javas
/dist/*
/html/*
.lacal
/node_moduels/**
**/*.svg
**/*.sh
/public/*
```



