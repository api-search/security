---
api_key_in: []
api_specs:
- filename: microsoft-yammer-files-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Files API
  slug: microsoft-yammer-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-files-api-openapi.yml
- filename: microsoft-yammer-groups-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Groups API
  slug: microsoft-yammer-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-groups-api-openapi.yml
- filename: microsoft-yammer-messages-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Messages API
  slug: microsoft-yammer-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-messages-api-openapi.yml
- filename: microsoft-yammer-networks-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Networks API
  slug: microsoft-yammer-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-networks-api-openapi.yml
- filename: microsoft-yammer-search-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Search API
  slug: microsoft-yammer-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-search-api-openapi.yml
- filename: microsoft-yammer-subscriptions-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Subscriptions API
  slug: microsoft-yammer-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-subscriptions-api-openapi.yml
- filename: microsoft-yammer-threads-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Threads API
  slug: microsoft-yammer-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-threads-api-openapi.yml
- filename: microsoft-yammer-topics-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Topics API
  slug: microsoft-yammer-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-topics-api-openapi.yml
- filename: microsoft-yammer-users-api-openapi.yml
  format: yaml
  label: Microsoft Yammer Users API
  slug: microsoft-yammer-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/openapi/microsoft-yammer-users-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Yammer Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Yammer secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Yammer
provider_slug: microsoft-yammer
scheme_count: 1
schemes:
- description: Yammer OAuth 2.0 legacy tokens or Microsoft Entra tokens. Delegated access only.
  flows:
  - authorizationUrl: https://www.yammer.com/dialog/oauth
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://www.yammer.com/oauth2/access_token.json
  name: OAuth2
  sources:
  - openapi/microsoft-yammer-openapi.yml
  type: oauth2
slug: microsoft-yammer-authentication
source_filename: microsoft-yammer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-yammer-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.yammer.com/dialog/oauth\n    tokenUrl: https://www.yammer.com/oauth2/access_token.json\n    scopes: 0\n  description: Yammer OAuth 2.0 legacy tokens or Microsoft Entra tokens. Delegated access only.\n  sources:\n  - openapi/microsoft-yammer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/authentication/microsoft-yammer-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Enterprise Social
- Microsoft
- Social Networking
- Viva Engage
- Yammer
---
