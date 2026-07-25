---
api_key_in: []
api_specs:
- filename: elementum-access-token-api-openapi.yml
  format: yaml
  label: Elementum Access Token API
  slug: elementum-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-access-token-api-openapi.yml
- filename: elementum-agents-api-openapi.yml
  format: yaml
  label: Elementum Agents API
  slug: elementum-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-agents-api-openapi.yml
- filename: elementum-apps-api-openapi.yml
  format: yaml
  label: Elementum Apps API
  slug: elementum-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-apps-api-openapi.yml
- filename: elementum-attachments-api-openapi.yml
  format: yaml
  label: Elementum Attachments API
  slug: elementum-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-attachments-api-openapi.yml
- filename: elementum-automations-api-openapi.yml
  format: yaml
  label: Elementum Automations API
  slug: elementum-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-automations-api-openapi.yml
- filename: elementum-comments-api-openapi.yml
  format: yaml
  label: Elementum Comments API
  slug: elementum-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-comments-api-openapi.yml
- filename: elementum-domains-api-openapi.yml
  format: yaml
  label: Elementum Domains API
  slug: elementum-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-domains-api-openapi.yml
- filename: elementum-elements-api-openapi.yml
  format: yaml
  label: Elementum Elements API
  slug: elementum-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-elements-api-openapi.yml
- filename: elementum-flows-api-openapi.yml
  format: yaml
  label: Elementum Flows API
  slug: elementum-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-flows-api-openapi.yml
- filename: elementum-groups-api-openapi.yml
  format: yaml
  label: Elementum Groups API
  slug: elementum-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-groups-api-openapi.yml
- filename: elementum-records-api-openapi.yml
  format: yaml
  label: Elementum Records API
  slug: elementum-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-records-api-openapi.yml
- filename: elementum-related-items-api-openapi.yml
  format: yaml
  label: Elementum Related-items API
  slug: elementum-related-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-related-items-api-openapi.yml
- filename: elementum-search-tables-api-openapi.yml
  format: yaml
  label: Elementum Search Tables API
  slug: elementum-search-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-search-tables-api-openapi.yml
- filename: elementum-skills-api-openapi.yml
  format: yaml
  label: Elementum Skills API
  slug: elementum-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-skills-api-openapi.yml
- filename: elementum-tables-api-openapi.yml
  format: yaml
  label: Elementum Tables API
  slug: elementum-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-tables-api-openapi.yml
- filename: elementum-users-api-openapi.yml
  format: yaml
  label: Elementum Users API
  slug: elementum-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-users-api-openapi.yml
- filename: elementum-views-api-openapi.yml
  format: yaml
  label: Elementum Views API
  slug: elementum-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-views-api-openapi.yml
- filename: elementum-watchers-api-openapi.yml
  format: yaml
  label: Elementum Watchers API
  slug: elementum-watchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-watchers-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Elementum Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Elementum secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Elementum
provider_slug: elementum
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.elementum.io/oauth/token
    tokenUrl_eu: https://api.eu.elementum.io/oauth/token
    token_ttl_seconds: 86400
  name: ClientCredentials
  sources:
  - openapi/elementum-openapi-original.json
  type: oauth2
slug: elementum-authentication
source_filename: elementum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/elementum-openapi-original.json\ndocs: https://docs.elementum.io/api-reference/api-introduction\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    OAuth 2.0 client-credentials only. Obtain a Client ID and Client Secret from User Settings >\n    OAuth (Create New Token > API Access) in the Elementum app; the secret is shown once. Exchange\n    them at the token endpoint using HTTP Basic Auth (client_id:client_secret, base64) with\n    grant_type=client_credentials, or a JSON/form body carrying client_id + client_secret +\n    grant_type. The returned Bearer access token is sent as `Authorization: Bearer <token>` and\n    expires after 24 hours. Service Accounts scope what an automation or agent token can do via\n    role-based permissions and data-access policies (no OAuth scope strings). US and EU regions.\nschemes:\n- name: ClientCredentials\n  type: oauth2\n  flows:\n  - flow:\
  \ clientCredentials\n    tokenUrl: https://api.elementum.io/oauth/token\n    tokenUrl_eu: https://api.eu.elementum.io/oauth/token\n    token_ttl_seconds: 86400\n    scopes: 0\n  sources:\n  - openapi/elementum-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/authentication/elementum-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- AI
- Automation
- Workflow
- Orchestration
- Agents
- Supply Chain
- No-Code
- Enterprise
- Snowflake
---
