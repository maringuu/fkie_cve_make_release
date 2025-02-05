<!--
SPDX-FileCopyrightText: 2024 Fraunhofer FKIE
SPDX-FileContributor: Marten Ringwelski <git@maringuu.de>

SPDX-License-Identifier: CC-BY-SA-4.0
-->
> Moved to https://github.com/fkie-cad/nvd-release-builder

# nvd-release-builder
A script and python package to create a release of
[nvd-json-data-feeds][nvd-json-data-feeds].

After installing using [poetry][poetry] the script can be used as follows:
```
Usage: nvd-release-builder [OPTIONS] FEEDS_PATH

  Creates release packages of the CVE data feeds released by FKIE-CAD [1]. The
  packages are put into FEEDS_PATH.

  [1]: https://github.com/fkie-cad/nvd-json-data-feeds

Options:
  --date [%Y-%m-%d]    Specifies the state of the database. Interpreted as a
                       date in UTC timezone. If not given implies '--fetch'.
  --fetch              Fetch the latest changes before proceeding.
  --xz-preset INTEGER  The xz compression preset level to use.
  --feed-name TEXT     The name of the feed to create. If not given, create
                       all feeds.
  --help               Show this message and exit.
```

Currently, there is no documentation for the python package but the
[nvd-release-builder](./nvd_release_builder/__main__.py) script
uses the package's api.

[nvd-json-data-feeds]: https://github.com/fkie-cad/nvd-json-data-feeds
[poetry]: https://python-poetry.org/
