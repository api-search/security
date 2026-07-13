---
api_key_in: []
api_specs:
- filename: microsoft-exchange-graph-mail-openapi.yml
  format: yaml
  label: Microsoft Graph Mail API
  slug: microsoft-graph-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-graph-mail-openapi.yml
- filename: microsoft-exchange-graph-calendar-openapi.yml
  format: yaml
  label: Microsoft Graph Calendar API
  slug: microsoft-graph-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-graph-calendar-openapi.yml
- filename: microsoft-exchange-graph-contacts-openapi.yml
  format: yaml
  label: Microsoft Graph Contacts API
  slug: microsoft-graph-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-graph-contacts-openapi.yml
- filename: microsoft-exchange-graph-people-openapi.yml
  format: yaml
  label: Microsoft Graph People API
  slug: microsoft-graph-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-graph-people-openapi.yml
- filename: microsoft-exchange-admin-api-openapi.yml
  format: yaml
  label: Exchange Online Admin API
  slug: exchange-online-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-admin-api-openapi.yml
- filename: microsoft-exchange-graph-import-export-openapi.yml
  format: yaml
  label: Microsoft Graph Mailbox Import Export API
  slug: microsoft-graph-mailbox-import-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-graph-import-export-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Exchange Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Exchange secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Exchange
provider_slug: microsoft-exchange
scheme_count: 2
schemes:
- description: OAuth 2.0 authorization with Microsoft identity platform
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-exchange-admin-api-openapi.yml
  - openapi/microsoft-exchange-graph-import-export-openapi.yml
  type: oauth2
- description: OAuth 2.0 authorization with Microsoft identity platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-exchange-graph-calendar-openapi.yml
  - openapi/microsoft-exchange-graph-contacts-openapi.yml
  - openapi/microsoft-exchange-graph-mail-openapi.yml
  - openapi/microsoft-exchange-graph-people-openapi.yml
  type: oauth2
slug: microsoft-exchange-authentication
source_filename: microsoft-exchange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-exchange-admin-api-openapi.yml, openapi/microsoft-exchange-graph-calendar-openapi.yml,\n  openapi/microsoft-exchange-graph-contacts-openapi.yml, openapi/microsoft-exchange-graph-import-export-openapi.yml,\n  openapi/microsoft-exchange-graph-mail-openapi.yml, openapi/microsoft-exchange-graph-people-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n    scopes: 1\n  description: OAuth 2.0 authorization with Microsoft identity platform\n  sources:\n  - openapi/microsoft-exchange-admin-api-openapi.yml\n  - openapi/microsoft-exchange-graph-import-export-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n\
  \    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 4\n  description: OAuth 2.0 authorization with Microsoft identity platform\n  sources:\n  - openapi/microsoft-exchange-graph-calendar-openapi.yml\n  - openapi/microsoft-exchange-graph-contacts-openapi.yml\n  - openapi/microsoft-exchange-graph-mail-openapi.yml\n  - openapi/microsoft-exchange-graph-people-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/authentication/microsoft-exchange-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Calendar
- Collaboration
- Contacts
- Email
- Enterprise
---
