# AWS Blocker

This simple bash script will retrieve the official list of AWS IP ranges, then block them all using iptables.

The script is safe to run multiple times. The AWS IP range list is updated periodically, so you may want to run this script as a cron.

## Requirements

You'll need *jq* to parse the JSON. This package is readily available in most Linux package managers.

## Usage

```
Usage: aws-blocker [POSITION] [REGIONS]...
```

Position is a nummeric value specifying the line number the INPUT chain target line will be inserted at. Defaults to 1.
Without any region arguments all IP ranges will by used.


Example:
```
aws-blocker 3 ap-southeast sa-east
```
