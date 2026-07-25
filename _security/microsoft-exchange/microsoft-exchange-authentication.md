---
api_key_in: []
api_specs:
- filename: microsoft-exchange-accepted-domains-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Accepted Domains API
  slug: microsoft-exchange-accepted-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-accepted-domains-api-openapi.yml
- filename: microsoft-exchange-attachments-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Attachments API
  slug: microsoft-exchange-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-attachments-api-openapi.yml
- filename: microsoft-exchange-calendars-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Calendars API
  slug: microsoft-exchange-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-calendars-api-openapi.yml
- filename: microsoft-exchange-contact-folders-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Contact Folders API
  slug: microsoft-exchange-contact-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-contact-folders-api-openapi.yml
- filename: microsoft-exchange-contacts-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Contacts API
  slug: microsoft-exchange-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-contacts-api-openapi.yml
- filename: microsoft-exchange-distribution-groups-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Distribution Groups API
  slug: microsoft-exchange-distribution-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-distribution-groups-api-openapi.yml
- filename: microsoft-exchange-events-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Events API
  slug: microsoft-exchange-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-events-api-openapi.yml
- filename: microsoft-exchange-mail-folders-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Mail Folders API
  slug: microsoft-exchange-mail-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-mail-folders-api-openapi.yml
- filename: microsoft-exchange-mailbox-discovery-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Mailbox Discovery API
  slug: microsoft-exchange-mailbox-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-mailbox-discovery-api-openapi.yml
- filename: microsoft-exchange-mailbox-export-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Mailbox Export API
  slug: microsoft-exchange-mailbox-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-mailbox-export-api-openapi.yml
- filename: microsoft-exchange-mailbox-folder-permissions-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Mailbox Folder Permissions API
  slug: microsoft-exchange-mailbox-folder-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-mailbox-folder-permissions-api-openapi.yml
- filename: microsoft-exchange-mailbox-import-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Mailbox Import API
  slug: microsoft-exchange-mailbox-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-mailbox-import-api-openapi.yml
- filename: microsoft-exchange-mailboxes-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Mailboxes API
  slug: microsoft-exchange-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-mailboxes-api-openapi.yml
- filename: microsoft-exchange-messages-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Messages API
  slug: microsoft-exchange-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-messages-api-openapi.yml
- filename: microsoft-exchange-organization-configuration-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Organization Configuration API
  slug: microsoft-exchange-organization-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-organization-configuration-api-openapi.yml
- filename: microsoft-exchange-people-api-openapi.yml
  format: yaml
  label: Microsoft Exchange People API
  slug: microsoft-exchange-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-people-api-openapi.yml
- filename: microsoft-exchange-scheduling-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Scheduling API
  slug: microsoft-exchange-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-scheduling-api-openapi.yml
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
