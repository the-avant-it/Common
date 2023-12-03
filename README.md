# Common.Common

Basic configuration for any VM

# Changelog

## 1.8.2

- Add unzip

## 1.8.1

- Honor ignore_package_installation_errors on apt update

## 1.8.0

- Add common.ignore_package_installation_errors variable

## 1.7.0

- Enable TCP BBR to improve network speed
- BREAKING CHANGE: Refac hostname module
- Add stress, iperf3, mtr

## 1.6.1

- Add hostname module

## 1.6.0

- Add dnspython

## 1.5.1

- Fix cache miss

## 1.5.0

- Add Install passlib
- Add optional common.cache_key

## 1.4.0

- Add optional common.enable_cache var and python-pexpect apt package

## 1.3.0

- Do not run the role if it executed recently

## 1.2.0

- Add traceroute for VK cloud
- Add retries for apt update for Russia

# Documentation for 1.8.2

## Variables

```yaml
common:
  # Optional
  enable_cache: yes
  # Optional
  cache_key: default
  # Optional
  ignore_package_installation_errors: no
```
