# OWASP CRS - phpMyAdmin Rule Exclusions Plugin

[![.github/workflows/integration.yml](https://github.com/coreruleset/phpmyadmin-rule-exclusions-plugin/actions/workflows/integration.yml/badge.svg)](https://github.com/coreruleset/phpmyadmin-rule-exclusions-plugin/actions/workflows/integration.yml)
[![.github/workflows/lint.yml](https://github.com/coreruleset/phpmyadmin-rule-exclusions-plugin/actions/workflows/lint.yml/badge.svg)](https://github.com/coreruleset/phpmyadmin-rule-exclusions-plugin/actions/workflows/lint.yml)

## Description

This plugin contains rule exclusions for [phpMyAdmin](https://www.phpmyadmin.net/),
a tool intended to handle the administration of MySQL over the Web, so it can be
run flawlessly togather with OWASP CRS (CRS).

## Installation

For full and up to date instructions for the different available plugin
installation methods, refer to [How to Install a Plugin](https://coreruleset.org/docs/concepts/plugins/#how-to-install-a-plugin)
in the official CRS documentation.

### Conditionally enable plugins for multi-application environments

For full and up to date instructions on how to conditionally enable/disable this plugin on a multisite environment, please refer to [Conditionally enable plugins for multi-application environments](https://coreruleset.org/docs/concepts/plugins/#conditionally-enable-plugins-for-multi-application-environments) in the official CRS documentation.

## Configuration

All settings can be done in file `plugins/phpmyadmin-rule-exclusions-config.conf`.

### tx.phpmyadmin-rule-exclusions-plugin_url_format

phpMyAdmin completely changed URL structure from version 5.1.0 so, if you are
running older version, set this setting to `old`. Otherwise, keep it to `v51`.

Default value: v51

## Testing

After the plugin is enabled, your phpMyAdmin instance should work without any
problems possibly caused by CRS (for example, false positives while blocking
requests). If you are still having any problems, please file a new issue on
[github](https://github.com/coreruleset/phpmyadmin-rule-exclusions-plugin).

## License

Copyright (c) 2022-2024 OWASP CRS project. All rights reserved.

The OWASP CRS and its official plugins are distributed
under Apache Software License (ASL) version 2. Please see the enclosed LICENSE
file for full details.
