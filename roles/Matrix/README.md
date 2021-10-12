## Values


| Key | Sub-key | Required | Default |
| - | - | - | - |
| host | hostname | Y | matrix |
| host | public_domain | Y | N/A |
| matrix | user | Y | matrix |
| matrix | user_home | Y | /srv/matrix |
| psql | application_user | Y | N/A |
| psql | application_password | Y | N/A |
| psql | application_database | Y | N/A |

Example below:
``` yaml
host:
  hostname: matrix
  public_domain: null.com

matrix:
  user: matrix
  user_home: /srv/matrix
  # These two create the server name and are used else where
  host: matrix
  domain: hanafin.pro

psql:
  application_user: matrix_user
  application_password: Password1!
  application_database: matrix
```

## ToDo
- Remove the use of host and domain under the matrix key and replace them with with host and domain under the host key

## Tested On:
  - CentOS Stream 8
