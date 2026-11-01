---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 9
method: searched
name: Radicale Authentication
name_suffix: Authentication
oauth_flows: []
overview: Radicale declares 9 security scheme(s) across its OpenAPI definitions.
provider_name: Radicale
provider_slug: radicale
scheme_count: 9
schemes:
- description: Authentication via htpasswd file
  type: htpasswd
- description: LDAP authentication
  type: ldap
- description: IMAP authentication
  type: imap
- description: Dovecot authentication
  type: dovecot
- description: PAM authentication
  type: pam
- description: OAuth2 server authentication (requires reverse proxy)
  type: oauth2
- description: Authentication via HTTP_REMOTE_USER header
  type: http_remote_user
- description: Authentication via HTTP_X_REMOTE_USER header
  type: http_x_remote_user
- description: Default deny all authentication (since 3.5.0)
  type: denyall
slug: radicale-authentication
source_filename: radicale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: searched\nsource: https://radicale.org/v3.html#authentication\nschemes:\n  - type: htpasswd\n    description: \"Authentication via htpasswd file\"\n  - type: ldap\n    description: \"LDAP authentication\"\n  - type: imap\n    description: \"IMAP authentication\"\n  - type: dovecot\n    description: \"Dovecot authentication\"\n  - type: pam\n    description: \"PAM authentication\"\n  - type: oauth2\n    description: \"OAuth2 server authentication (requires reverse proxy)\"\n  - type: http_remote_user\n    description: \"Authentication via HTTP_REMOTE_USER header\"\n  - type: http_x_remote_user\n    description: \"Authentication via HTTP_X_REMOTE_USER header\"\n  - type: denyall\n    description: \"Default deny all authentication (since 3.5.0)\""
source_yaml_url: https://artifacts.apis.io/radicale/authentication/radicale-authentication.yml
summary_line: 9 schemes
tags:
- Company
- CalDAV
- CardDAV
- OpenSource
- Python
- Calendar
---
