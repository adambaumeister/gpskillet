# GlobalProtect Setup Skillet
## Test matrix
| Version(branch)          | 8.0           | 8.1(panos_v8.1)  | 9.0(master) |
| ------------- |:-------------:| -----:| --- |
| Panorama     | N | N| N |
| Panos      | N| Y| Y |


## Description
Sets up a basic GlobalProtect configuration with one portal, one EGW, and LDAP authentication.

## Prequisites 

 * SSL Profiles (PORTAL_SSL_PROFILE and EGW_SSL_PROFILE) already configured on firewall 
 * Reachable IP addresses (GP_PORTAL_IP and GP_EXTERNAL_GW_ADDR)
 * A YAML config file populated with all relevant variables.
 
## Use
See here: https://github.com/adambaumeister/skilletcli

```bash
skilletcli --repository gpskillet --repopath https://github.com/adambaumeister/gpskillet.git
```
