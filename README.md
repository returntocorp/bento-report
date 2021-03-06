# bento-report

[![r2c community slack](https://img.shields.io/badge/r2c_slack-join-brightgreen?style=for-the-badge&logo=slack&labelColor=4A154B)](https://join.slack.com/t/r2c-community/shared_invite/enQtNjU0NDYzMjAwODY4LWE3NTg1MGNhYTAwMzk5ZGRhMjQ2MzVhNGJiZjI1ZWQ0NjQ2YWI4ZGY3OGViMGJjNzA4ODQ3MjEzOWExNjZlNTA)

This script configures [Bento](https://github.com/returntocorp/bento)
for commonly used security reporting setups.

## Installation

```
$ curl -Lo /usr/local/bin/bento-report-init https://git.io/bento-report-init
$ chmod +x /usr/local/bin/bento-report-init
```

## Usage

```
$ bento-report-init
```

to fetch the default security reporting configuration.
You can select an alternative one by specifying its name:

```
$ bento-report-init --config django
```

or if its your own local config template, its path:

```
$ bento-report-init --config ~/.bento-report-configs/lukes-special-edition-bento
```

Assuming that the provided directory looks like this:

```
~/.bento-report-configs
└── lukes-special-edition-bento
    ├── .bentoignore
    └── config.yml
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md)
