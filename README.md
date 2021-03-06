# dpkg-history
_maintained by Warwalrux_

## About

Proposed as a debian equivalent to [`yum-history`](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/6/html/deployment_guide/sec-yum-transaction_history), `dpkg-history` is capable of browsing through a transactional view of package maintenance history, as documented by dpkg.

![Basic Usage](https://github.com/warwalrux/apt-history/raw/main/doc/screenshots/1.png)

## Usage

##### **dpkg-history** [-h] [--debug] [ --list | --info _ID_ | --inspect _ID_ | --redo _ID_ | --undo _ID_ ]

```
optional arguments:
  -h, --help         show this help message and exit
  --debug            debug switch
  --list             Show dpkg transactions
  --info INFO        Show transaction report by ID
  --inspect INSPECT  Show detailed transaction data
  --redo REDO        Redo transaction by ID
  --undo UNDO        Undo transaction by ID
```

## Installation

For now the entire repo can be extracted into `/usr/share/lib`.
the `dpkg-history` executable can be symbolically linked from
`/usr/share/lib` to `/usr/bin` and then used globally.
