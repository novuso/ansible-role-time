# Ansible Role: Time

[![MIT License](http://img.shields.io/badge/license-MIT-003399.svg)](http://opensource.org/licenses/MIT)

An Ansible role that manages timezone and NTP on Ubuntu 14.04

## Requirements

None

## Role Variables

Ansible variables are listed here along with their default values:

`time_system_timezone` sets the system timezone.

    time_system_timezone: "UTC"

`time_ntp_enabled` flags whether or not to enable NTP.

    time_ntp_enabled: true

## Dependencies

None

## Example Playbook

    ---
    - hosts: all
      vars:
      - time_system_timezone: "America/Chicago"
      roles:
      - novuso.time

## License

This is released under the [MIT license](http://opensource.org/licenses/MIT).
