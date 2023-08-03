#### 安装包

```javas
npm add @commitlint/config-conventional @commitlint/cli -D
```

#### 配置commitlint.config.cjs文件

```javas
module.exports = {
  ignores: [(commit) => commit.includes("init")],
  extends: ["@commitlint/config-conventional"],
  rules: {
    "body-leading-blank": [2, "always"],
    "footer-leading-blank": [1, "always"],
    "header-max-length": [2, "always", 108],
    "subject-empty": [2, "never"],
    "type-empty": [2, "never"],
    "subject-case": [0],
  },
};
```

#### 在package.json文件中添加配置

```json
"script":{
    "commitlint":"commitlint --config commitlint.config.cjs -e -V"
}
```

