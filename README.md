# Meson for Visual Studio Code

This extension provides support for [Meson](http://mesonbuild.com/) in
[Visual Studio Code](https://code.visualstudio.com/). This language grammar was
based on the grammar found in the
[atom extension](https://github.com/TingPing/language-meson) from
[Patrick Griffis](https://github.com/TingPing), but has since been added onto to
support more features, including code from the VSCode
[grammar](https://github.com/microsoft/vscode/blob/main/extensions/python/syntaxes/MagicPython.tmLanguage.json)
for Python.

Meson logo by [Jussi Pakkanen](https://github.com/jpakkane),
[licensed for use by this project](http://mesonbuild.com/legal.html). Icons from
the [Material Design Icons](https://materialdesignicons.com/) project.

## Features

- Syntax Highlighting
- Automatic Task Provider
- Code Snippets
- Linting[^0]
- Formatting[^1]
- Generate environment file to be used in launch.json:
  `"envFile": "${workspaceFolder}/${config:mesonbuild.buildFolder}/meson-vscode.env"`
  See [Meson devenv](https://mesonbuild.com/Commands.html#devenv)
- Configure Intellisense to use the `compile_commands.json` generated by Meson
- Provide an Intellisense C/C++ configuration to use the `meson-info`
  introspection files:
  `"C_Cpp.default.configurationProvider": "mesonbuild.mesonbuild"`

## New Extension ID

If you come from a previous installation, please make sure you are on the
**mesonbuild.mesonbuild** extension. There are 3 variants/versions of this
extension on the store, and only that one is released from this repository.

[^0]:
    Requires an installation of
    [mesonlsp](https://github.com/JCWasmx86/mesonlsp) or
    [muon](https://muon.build).

[^1]: Requires an installation of muon or meson >= 1.5.0
