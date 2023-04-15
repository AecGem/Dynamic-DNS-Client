# Dynamic-DNS-Client
A simple script that sends an IP update request to a Dynamic DNS Registry at a regular interval. The script requires the Python requests package, so run `pip install requests` before running this script.

## Setup
In order to set up the Dynamic DNS client, you have to change a few variables in the script.

### host
Basically change this to the prefix of the domain you wish to update. For most uses the default value `@` works fine. Otherwise you can specify a wildcard `*` or a specific prefix (`www`, `info`, `ww2`, etc.)

### domain_name
The domain you are updating, without any prefix. Ex: `google.ca`

### ddns_password
The password provided to you by your Dynamic DNS provider for your domain.

### update_frequency
The interval, in seconds, that will pass between updates. For example, setting this to 60 will send an update request once every minute (60 seconds.)
