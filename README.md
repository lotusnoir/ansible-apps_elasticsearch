# ansible-apps_elasticsearch

[![Galaxy Role](https://img.shields.io/badge/galaxy-apps_elasticsearch-purple?style=flat)](https://galaxy.ansible.com/lotusnoir/apps_elasticsearch)
[![Version](https://img.shields.io/github/release/lotusnoir/ansible-apps_elasticsearch.svg)](https://github.com/lotusnoir/ansible-apps_elasticsearch/releases/latest)
[![GitHub repo size](https://img.shields.io/github/repo-size/lotusnoir/ansible-apps_elasticsearch?color=orange&style=flat)](https://galaxy.ansible.com/lotusnoir/apps_elasticsearch)
[![downloads](https://img.shields.io/ansible/role/d/lotusnoir/apps_elasticsearch)](https://galaxy.ansible.com/lotusnoir/apps_elasticsearch)
[![License](https://img.shields.io/badge/license-Apache--2.0-brightgreen?style=flat)](https://opensource.org/licenses/Apache-2.0)

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Description](#description)
- [Requirements](#requirements)
- [Role variables](#role-variables)
- [Examples](#examples)
- [License](#license)
- [Author Information](#author-information)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Description

Deploy and configure elasticsearch

tested to deploy elasticsearch 9.x.

install time with repo = 1/run 145.73s -  2/run 8.56s
install time with src / local = 1/run  30.75s - 2/run 10.73s
install time with src / internet / host = 1/run 30.39s - 2/run 11.23s
install time with src / internet / localhost = 1/run 33.59s - 2/run 11.47s


## Requirements

none

## Role variables

See [variables](/defaults/main.yml) for more details.

## Examples

        ---
        - hosts: apps_elasticsearch
          become: true
          become_method: sudo
          gather_facts: true
          roles:
            - role: ansible-apps_elasticsearch

## Grafana Dashboard

You can find a grafana dashboard [here](https://grafana.com/grafana/dashboards/)

## License

This project is licensed under Apache License. See [LICENSE](/LICENSE) for more details.

## Author Information

- [Philippe LEAL](https://github.com/lotusnoir)
