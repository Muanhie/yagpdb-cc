# Automod Ping

Sends a ping to a mod role after every message from Discord's built-in automod.

## Setup
Trigger Type: Regex<br />
Trigger: `.*`

### Configuring to support additional mod roles
When adding IDs of more roles, ensure line 16 has been updated to include the Value label.
_e.g. If a label was added of ID 'xxxxxxxxxxxxxxxxxxx' under $ownderRole, it would be changed to include another (hasRoleID $) within the line; this can be repeated for as many staff roles._
```
{{ if not (or (hasRoleID $reportRole) (hasRoleID $modRole) (hasRoleID $adminRole) (hasRoleID $botRole) (hasRoleID $ownerRole) ) }}
```

### Output
![image](https://user-images.githubusercontent.com/97837239/179002730-2759d05d-2e0c-4a46-8962-4aae5b8719bd.png)
