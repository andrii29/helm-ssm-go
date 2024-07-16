# Helm SSM Replacer Plugin

This plugin replaces placeholders in the format `{{ssm /path/to/parameter region}}` with actual values from AWS SSM Parameter Store.

## Installation

To install the plugin, run the following command:

```sh
helm plugin install https://github.com/sport-labs-group/helm-ssm-go
```
To install specific version of plugin or architecture, run the following commands
```sh
export VERSION='0.5.0'
export ARCH='arm64
helm plugin install https://github.com/sport-labs-group/helm-ssm-go
```
## Usage
```sh
helm ssm -f values.yaml
```
Command reads data from values.yaml file print to stdout content with replaced ssm params

## Credentials
Use [environment variables](https://docs.aws.amazon.com/cli/v1/userguide/cli-configure-envvars.html) `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` or any other supported way to [configure](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html) aws cli
