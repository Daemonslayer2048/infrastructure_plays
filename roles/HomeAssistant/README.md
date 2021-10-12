## Values
This implementation uses a MariaDB backend so the following values are required under the mysql key.

| Key | Sub-key | Required | Default |
| - | - | - | - |
| host | hostname | Y | hass |
| host | public_domain | Y | N/A |
| homeassistant | user_home | N | /srv/homeassistant |
| mysql | root_password | Y | N/A |
| mysql | application_database | Y | N/A |
| mysql | application_user | Y | N/A |
| mysql | application_password | Y | N/A |

Example below:
``` yaml
host:
  hostname: hass
  public_domain: null.com

homeassistant:
  user_home: /srv/homeassistant

# Please do not keep this. This is intended to show values needed.
mysql:
  root_password: Password1!
  application_database: homeassistant
  application_user: hass
  application_password: Password1!

```

## ToDo
- Set hostname to the same as the public host.  
  Terragrunt uses hass as the hostname but ansible uses homeasiststn

## Tested On:
  - CentOS Stream 8
  - RHEL 8
