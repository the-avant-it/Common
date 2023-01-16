# Common.Common

Basic configuration for any VM

# Changelog

## V1.8.2

- Add unzip

## V1.8.1

- Honor ignore_package_installation_errors on apt update

## V1.8.0

- Add common.ignore_package_installation_errors variable

## V1.7.0

- Enable TCP BBR to improve network speed
- BREAKING CHANGE: Refac hostname module
- Add stress, iperf3, mtr

## V1.6.1

- Add hostname module

## V1.6.0

- Add dnspython

## V1.5.1

- Fix cache miss

## V1.5.0

- Add Install passlib
- Add optional common.cache_key

## V1.4.0

- Add optional common.enable_cache var and python-pexpect apt package

## V1.3.0

- Do not run the role if it executed recently

## V1.2.0

- Add traceroute for VK cloud
- Add retries for apt update for Russia