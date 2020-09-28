# IAM_policies


Description
================================================================================
This project/repository contains IAM policies needed for Aviatrix features accross cloud providers/vendors, AWS, Azure and GCP.


References
================================================================================
https://docs.aviatrix.com


Contributors
================================================================================


AWS IAM Files Naming Convention
--------------------------------------------------------------------------------
* Always start with the string "aviatrix" with all lower cases
* Always include the string "-iam-policy" so it's clear/straightforward for people to understand what type this file is for
* Always use dashes '-' instead of whitespaces or underscores


Format
--------------------------------------------------------------------------------

```
aviatrix-<NAME_OF_AVIATRIX_FEATURE>-iam-policy-<AWS_ACCOUNT_TYPE>-<API_PERMISSION_REQUSTER>.json
```

**<NAME_OF_AVIATRIX_FEATURE>**
Valid values are: (snake-style lower cases)
    + access-account
    + multi-cloud-transit
    + aws-tgw-orchestrator
    + firewall-network
    + cloudwan
    + peering
    + site2cloud
    + openvpn
    + stateful-firewall
    + egresscontrol
    + aws-guardduty
    + public-subnet
    + private-s3
    + fqdn
    + vpc
    + upgrade
    + backup-and-restore
    + controller-migration
    + security-patches
    + software-patches
    + tracelog
    + diagnostics
    + flightpath


**<AWS_ACCOUNT_TYPE>**
Currently, the valid values are: (camel cases)
    + "Primary"
    + "Secondary"


**<API_PERMISSION_REQUSTER>**
Currently, the valid values are: (camel cases)
    + "Controller"
    + "Gateway"
    + "CrossAccount"
