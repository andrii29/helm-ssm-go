# Helm SSM Replacer Plugin

This plugin replaces placeholders in the format `{{ssm /path/to/parameter region}}` with actual values from AWS SSM Parameter Store.

## Installation

To install the plugin, run the following command:

```sh
helm plugin install https://github.com/andrii29/helm-ssm-go
```
To install specific version of plugin or architecture, run the following commands
```sh
export VERSION='0.2.0'
export ARCH='arm64
helm plugin install https://github.com/andrii29/helm-ssm-go
```
## Usage
```sh
helm ssm -f values.yaml
```
Command reads data from values.yaml file print to stdout content with replaced ssm params
