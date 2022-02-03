Steps:

1) install vscode eslint extension by microsoft

2) create $.eslintrc.json$ file

3) copy eslintrc config from [Safe-Customer-App](https://github.com/orocorp/safe/tree/dev).

4) run command 

```bash
npm i eslint eslint-plugin-eslint-plugin @babel/eslint-parser @babel/eslint-plugin eslint-plugin-jsx eslint-plugin-prefer-optional-chaining eslint-plugin-react --save-dev
```

5) open vscode settings > goto extensions section > goto eslint section and enable these

- Eslint always show status should be enabled.
- Eslint: Debug should be enabled
- Eslint: Enable, should be enabled
- Eslint > Format: Enable, should be enabled
- Eslint > Lint task, should be enabled

6) Open settings.json. It should have eslint properties used in this.

```bash
{
    "workbench.colorTheme": "Visual Studio Light",
    "diffEditor.ignoreTrimWhitespace": false,
    "git.suggestSmartCommit": false,
    "eslint.enable": true,
    "eslint.format.enable": true,
    "eslint.debug": true,
    "debug.javascript.autoAttachFilter": "onlyWithFlag",
    "editor.tabSize": 2,
    "editor.suggestSelection": "first",
    "vsintellicode.modify.editor.suggestSelection": "automaticallyOverrodeDefaultValue",
    "files.exclude": {
        "**/.classpath": true,
        "**/.project": true,
        "**/.settings": true,
        "**/.factorypath": true
    },
    "eslint.lintTask.enable": true,
    "eslint.alwaysShowStatus": true
}
```

7) Above steps can change with time. Please google accordingly.

8) Finally restart vscode.(Close it and open again). Files should be linted now, you can check by adding some bad code.

9) If not linting, click on eslint in the vscode status bar(at the bottom). There should be some label called eslint. If not visible wait for sometime or try restarting vscode. Extension should be installed and previous steps must be performed.

10) On clicking eslint in status bar, scroll completely bottom. You should see Linting complete text. If not some error will be logged. Debug accordingly, either install extra packages or google.
