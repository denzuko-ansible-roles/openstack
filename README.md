# Openstack [![Open in Cloud9](https://img.shields.io/badge/Open%20in-Cloud9-blue.svg?style=flat-square)](https://c9.io/auth/github?r=https%3A%2F%2Fc9.io%2Fopen%2F%3Fclone_url%3Dhttps%253A%252F%252Fgithub.com%252Fdenzuko-ansible-roles%252Fopenstack.git) [![Analytics](https://ga-beacon.appspot.com/UA-110571074-1/denzuko/ansible-roles/openstack?flat)](https://github.com/denzuko-ansible-roles/openstack) [![CiCD](https://img.shields.io/travis/denzuko-ansible-roles/openstack.svg?style=flat-square)](https://travis-ci.org/denzuko-ansible-roles/openstack)

Installs latest version of openstack

## Installation
$ ``` ansible-galaxy install denzuko-ansible-roles.openstack ```

## Requirements
* `ansible=>2.2`
* `Linux server`

## Supports
* MySQL backend
* fullstack of openstack
* Ubuntu, Debian
* RHEL, CentOS

## Files
This module Installs [devstack](https://wiki.openstack.org/wiki/DevStack) based
on config values passed along via a dictionary named `config`.


## Configuration

| Name | Description  | Schema  |Defaults |
|---|---|---|---|
| floating_range| Available IP Pool for public access | CIDR | Interactive prompt |
| fix_range | Internal IP Pool for virtual machines | CIDR | Interactive prompt |
| fix_network_size | Number of ip addresses | INT | Interactive prompt |
| flat_interface | Main networking interface | STR | Interactive prompt |
| admin_secret | Administrator's password | STR | Interactive prompt |
| service_secret | Web Service password | STR | Same as admin_secret |
| broker_secret | Rabbit user's password | STR | Interactive prompt |
| database_secret | Database user's password | STR | Interactive prompt |
| swift_replicas | Number of swift replicas to spawn | INT | 1 |
