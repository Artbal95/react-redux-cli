oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![Downloads/week](https://img.shields.io/npm/dw/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![License](https://img.shields.io/npm/l/oclif-hello-world.svg)](https://github.com/oclif/hello-world/blob/main/package.json)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g react-redux-cli
$ react-redux-cli COMMAND
running command...
$ react-redux-cli (--version)
react-redux-cli/0.0.0 linux-x64 node-v14.18.2
$ react-redux-cli --help [COMMAND]
USAGE
  $ react-redux-cli COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`react-redux-cli hello PERSON`](#react-redux-cli-hello-person)
* [`react-redux-cli hello world`](#react-redux-cli-hello-world)
* [`react-redux-cli help [COMMAND]`](#react-redux-cli-help-command)
* [`react-redux-cli plugins`](#react-redux-cli-plugins)
* [`react-redux-cli plugins:install PLUGIN...`](#react-redux-cli-pluginsinstall-plugin)
* [`react-redux-cli plugins:inspect PLUGIN...`](#react-redux-cli-pluginsinspect-plugin)
* [`react-redux-cli plugins:install PLUGIN...`](#react-redux-cli-pluginsinstall-plugin-1)
* [`react-redux-cli plugins:link PLUGIN`](#react-redux-cli-pluginslink-plugin)
* [`react-redux-cli plugins:uninstall PLUGIN...`](#react-redux-cli-pluginsuninstall-plugin)
* [`react-redux-cli plugins:uninstall PLUGIN...`](#react-redux-cli-pluginsuninstall-plugin-1)
* [`react-redux-cli plugins:uninstall PLUGIN...`](#react-redux-cli-pluginsuninstall-plugin-2)
* [`react-redux-cli plugins update`](#react-redux-cli-plugins-update)

## `react-redux-cli hello PERSON`

Say hello

```
USAGE
  $ react-redux-cli hello [PERSON] -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/hello/index.ts](https://github.com/Artbal95/react-redux-cli.git/react-redux-cli/blob/v0.0.0/dist/commands/hello/index.ts)_

## `react-redux-cli hello world`

Say hello world

```
USAGE
  $ react-redux-cli hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ react-redux-cli hello world
  hello world! (./src/commands/hello/world.ts)
```

## `react-redux-cli help [COMMAND]`

Display help for react-redux-cli.

```
USAGE
  $ react-redux-cli help [COMMAND] [-n]

ARGUMENTS
  COMMAND  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for react-redux-cli.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.1.10/src/commands/help.ts)_

## `react-redux-cli plugins`

List installed plugins.

```
USAGE
  $ react-redux-cli plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ react-redux-cli plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.0.11/src/commands/plugins/index.ts)_

## `react-redux-cli plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ react-redux-cli plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ react-redux-cli plugins add

EXAMPLES
  $ react-redux-cli plugins:install myplugin 

  $ react-redux-cli plugins:install https://github.com/someuser/someplugin

  $ react-redux-cli plugins:install someuser/someplugin
```

## `react-redux-cli plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ react-redux-cli plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ react-redux-cli plugins:inspect myplugin
```

## `react-redux-cli plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ react-redux-cli plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ react-redux-cli plugins add

EXAMPLES
  $ react-redux-cli plugins:install myplugin 

  $ react-redux-cli plugins:install https://github.com/someuser/someplugin

  $ react-redux-cli plugins:install someuser/someplugin
```

## `react-redux-cli plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ react-redux-cli plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Links a plugin into the CLI for development.

  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.

EXAMPLES
  $ react-redux-cli plugins:link myplugin
```

## `react-redux-cli plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ react-redux-cli plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ react-redux-cli plugins unlink
  $ react-redux-cli plugins remove
```

## `react-redux-cli plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ react-redux-cli plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ react-redux-cli plugins unlink
  $ react-redux-cli plugins remove
```

## `react-redux-cli plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ react-redux-cli plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ react-redux-cli plugins unlink
  $ react-redux-cli plugins remove
```

## `react-redux-cli plugins update`

Update installed plugins.

```
USAGE
  $ react-redux-cli plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```
<!-- commandsstop -->
