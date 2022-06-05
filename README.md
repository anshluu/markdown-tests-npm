---
title: npm-ping
section: 1
description: Ping npm registry
redirect_from:
  - /cli/ping
  - /cli/ping.html
  - /cli/commands/ping
  - /cli-commands/ping
  - /cli-commands/ping.html
  - /cli-commands/npm-ping
github_repo: npm/cli
github_branch: latest
github_path: docs/content/commands/npm-ping.md
---

### Synopsis

<!-- AUTOGENERATED USAGE DESCRIPTIONS START -->
<!-- automatically generated, do not edit manually -->
<!-- see lib/commands/ping.js -->

```bash
npm ping
```

<!-- automatically generated, do not edit manually -->
<!-- see lib/commands/ping.js -->

<!-- AUTOGENERATED USAGE DESCRIPTIONS END -->

Note: This command is unaware of workspaces.

### Description

Ping the configured or given npm registry and verify authentication.
If it works it will output something like:

```bash
npm notice PING https://registry.npmjs.org/
npm notice PONG 255ms
```
otherwise you will get an error:
```bash
npm notice PING http://foo.com/
npm ERR! code E404
npm ERR! 404 Not Found - GET http://www.foo.com/-/ping?write=true
```

### Configuration

<!-- AUTOGENERATED CONFIG DESCRIPTIONS START -->
<!-- automatically generated, do not edit manually -->
<!-- see lib/utils/config/definitions.js -->
#### `registry`

* Default: "https://registry.npmjs.org/"
* Type: URL

The base URL of the npm registry.

<!-- automatically generated, do not edit manually -->
<!-- see lib/utils/config/definitions.js -->

<!-- AUTOGENERATED CONFIG DESCRIPTIONS END -->

### See Also

* [npm doctor](/main/content/cli/v8/commands/npm-doctor.md)
* [npm config](/cli/v8/commands/npm-config)
* [npmrc](/cli/v8/configuring-npm/npmrc)
