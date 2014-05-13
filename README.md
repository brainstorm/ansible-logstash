ansible-logstash
=================

Ansible Playbook to deploy a vanilla Logstash 1.4.x install. Forked from mstrisonline (for logstash 1.3.x):

https://github.com/mstrisoline/ansible-logstash-play

## What this role does

This is a barebones ansible role to pull logstash from the official elasticsearch repos on debian based distributions.

## Quickstart

If you have hosts defined in your current ansible installation:

    ansible-playbook -i hosts/production roles/logstash/logstash.yml

For a one-off given an IP address (mind the final comma):

	ansible-playbook roles/logstash/logstash.yml -i 10.0.100.50,

## What this role does not do

It does not configure logstash. There are many complex and different ways to configure it, so I leave
that up to the experties of the end user to adjust the config the way they see fit. Does not set logstash
to start at boot.

## Working Distros

This has been tested and working with Ubuntu 14.04

### Feedback and constructive critisim is much appreciated.
