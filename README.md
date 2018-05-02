# Weblog helper v0.01

## Description

The weblog helper is a tool to filter ipaddress and ipaddress cidr for analyzing webserver logs. 

## Requirements

``bash``

``ipcalc v0.41``

# Usage

## General Command

```

$ sh weblog_helper

Usage: weblog_helper [option] <ADDRESS> [option] <FILE>
Usage: weblog_helper [option] <ADDRESS>

```

## Help Command

```
$ sh weblog_helper -h

Usage: weblog_helper [option] <ADDRESS> [option] <FILE>
Usage: weblog_helper [option] <ADDRESS>

Options:
    -i --ip        IP ADDRESS or CIDR ADDRESS
    -f --file      Input file default: source.txt
    -h --help      Usage help
```

## Applicable Command (with source.txt in PWD)

Modify web server logs file to source.txt or rename FILE variable as per you requirement

```
$ sh weblog_helper --ip 10.0.0.0/24
```

## Applicable Command (with specific file in PWD)

You do not need to modify code at all, just use option ``-f`` or ``--file``

```
sh weblog_helper --ip 10.0.0.0/24 -f filename
```
