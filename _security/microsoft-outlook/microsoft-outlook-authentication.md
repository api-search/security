---
api_key_in: []
api_specs:
- filename: microsoft-graph-mail-api-openapi.yml
  format: yaml
  label: Microsoft Graph Mail API
  slug: microsoft-graph-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/openapi/microsoft-graph-mail-api-openapi.yml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Calendar API
  slug: microsoft-graph-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Contacts API
  slug: microsoft-graph-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Tasks API
  slug: microsoft-graph-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph People API
  slug: microsoft-graph-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Change Notifications API
  slug: microsoft-graph-change-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Focused Inbox API
  slug: microsoft-graph-focused-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Mail Rules API
  slug: microsoft-graph-mail-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Categories API
  slug: microsoft-graph-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Outlook Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Outlook secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Outlook
provider_slug: microsoft-outlook
scheme_count: 1
schemes:
- description: Microsoft identity platform OAuth 2.0 authorization. Supports delegated (user) and application permissions.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-graph-mail-api-openapi.yml
  type: oauth2
slug: microsoft-outlook-authentication
source_filename: microsoft-outlook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-graph-mail-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 6\n  description: Microsoft identity platform OAuth 2.0 authorization. Supports delegated (user)\n    and application permissions.\n  sources:\n  - openapi/microsoft-graph-mail-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/authentication/microsoft-outlook-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Calendar
- Contacts
- Email
- Enterprise
- Microsoft
- Office 365
- Productivity
---
