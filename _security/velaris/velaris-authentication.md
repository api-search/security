---
api_key_in: []
api_specs:
- filename: velaris-activity-api-openapi.yml
  format: yaml
  label: Velaris Activity API
  slug: velaris-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-activity-api-openapi.yml
- filename: velaris-attribute-change-log-api-openapi.yml
  format: yaml
  label: Velaris Attribute Change Log API
  slug: velaris-attribute-change-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-attribute-change-log-api-openapi.yml
- filename: velaris-currencies-api-openapi.yml
  format: yaml
  label: Velaris Currencies API
  slug: velaris-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-currencies-api-openapi.yml
- filename: velaris-custom-objects-api-openapi.yml
  format: yaml
  label: Velaris Custom Objects API
  slug: velaris-custom-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-custom-objects-api-openapi.yml
- filename: velaris-entity-management-v1-api-openapi.yml
  format: yaml
  label: Velaris Entity Management V1 API
  slug: velaris-entity-management-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-entity-management-v1-api-openapi.yml
- filename: velaris-entity-management-v2-api-openapi.yml
  format: yaml
  label: Velaris Entity Management V2 API
  slug: velaris-entity-management-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-entity-management-v2-api-openapi.yml
- filename: velaris-field-definitions-api-openapi.yml
  format: yaml
  label: Velaris Field Definitions API
  slug: velaris-field-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-field-definitions-api-openapi.yml
- filename: velaris-integrations-api-openapi.yml
  format: yaml
  label: Velaris Integrations API
  slug: velaris-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-integrations-api-openapi.yml
- filename: velaris-lifecycles-api-openapi.yml
  format: yaml
  label: Velaris Lifecycles API
  slug: velaris-lifecycles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-lifecycles-api-openapi.yml
- filename: velaris-notes-api-openapi.yml
  format: yaml
  label: Velaris Notes API
  slug: velaris-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-notes-api-openapi.yml
- filename: velaris-surveys-api-openapi.yml
  format: yaml
  label: Velaris Surveys API
  slug: velaris-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-surveys-api-openapi.yml
- filename: velaris-tasks-api-openapi.yml
  format: yaml
  label: Velaris Tasks API
  slug: velaris-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-tasks-api-openapi.yml
- filename: velaris-ticketing-api-openapi.yml
  format: yaml
  label: Velaris Ticketing API
  slug: velaris-ticketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-ticketing-api-openapi.yml
- filename: velaris-users-api-openapi.yml
  format: yaml
  label: Velaris Users API
  slug: velaris-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Velaris Authentication
name_suffix: Authentication
oauth_flows: []
overview: Velaris secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Velaris
provider_slug: velaris
scheme_count: 2
schemes:
- description: 'User-scoped access token. Header: Authorization: Bearer {access_token}. Create under Profile > Security > Access token.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/velaris-openapi.yml
  type: http
- description: Legacy. Base64(username:password). Not available for SSO/MFA tenants.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/velaris-openapi.yml
  type: http
slug: velaris-authentication
source_filename: velaris-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.velaris.io/ (auth section) + openapi/velaris-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'User-scoped access token. Header: Authorization: Bearer {access_token}. Create under Profile > Security\n    > Access token.'\n  sources:\n  - openapi/velaris-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Legacy. Base64(username:password). Not available for SSO/MFA tenants.\n  sources:\n  - openapi/velaris-openapi.yml\ndocs: https://developers.velaris.io/\ndetail: 'Two options: (1) Token-based - any user creates a user-scoped API token in-app under Profile > Security\n  > Access token, sent as Authorization: Bearer {access_token}; works for SSO and non-SSO tenants. (2) Basic authentication\n  (legacy) - Base64(username:password) of an administrator-privileged user, sent as Authorization: Basic {token};\n  not available\
  \ for SSO-enabled tenants.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/authentication/velaris-authentication.yml
summary_line: http · 2 schemes
tags:
- Customer Success
- Artificial Intelligence
- Software-as-a-Service
- Customer Data
- CRM
- Analytics
- Automation
- Company
---
