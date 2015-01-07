# AWS Blocker

This simple bash script will retrieve the official list of AWS IP ranges, then block them all using iptables.

The script is safe to run multiple times. The AWS IP range list is updated periodically, so you may want to run this script as a cron.

## Requirements

You'll need *jq* to parse the JSON. This package is readily available in most Linux package managers.

## Usage

It doesn't take any arguments. Just run it.
