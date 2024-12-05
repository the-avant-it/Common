# Common.Common

Basic configuration for any VM

# Changelog

## 1.12.0

- Add Setup delete old logs cron

## 1.11.2

- Add optional variables for set timezones
```yaml
common:
  # Optional
  timezone: "Europe/Moscow"
```
To find your time zone, use:
```
timedatectl list-timezones
```
- Force add "localhost" resolves to 127.0.0.1
- Also add variables for language:
```yaml
  language:
    setup: false
    locale_package: language-pack-en
    system_locale: en_US.utf8 
```
https://sourceware.org/glibc/wiki/Locales

## 1.10.1

- Add Unminimize OS trask

## 1.9.6

- Add skip_sysctl var (should be set to true when running in container!)
- Fix lint errors 
- Fix "Stop snapd service"

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

# Documentation for 1.9.0

## Variables

```yaml
common:
  # Optional
  enable_cache: yes
  # Optional
  cache_key: default
  # Optional
  ignore_package_installation_errors: no
  # Optional. False by default. Should be set to true when aplying role to container!
  skip_sysctl: false
```
