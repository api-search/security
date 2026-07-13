---
api_key_in:
- header
api_specs:
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Inventory Items API
  slug: quartzy-inventory-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Order Requests API
  slug: quartzy-order-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Types API
  slug: quartzy-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Labs API
  slug: quartzy-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Webhooks API
  slug: quartzy-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Quartzy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Quartzy secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Quartzy
provider_slug: quartzy
scheme_count: 2
schemes:
- description: Per-user AccessToken generated in Quartzy under Profile > Access Tokens and sent in the Access-Token header.
  in: header
  name: accessToken
  parameter: Access-Token
  sources:
  - openapi/quartzy-openapi.yml
  type: apiKey
- description: OAuth2 authorization for Quartzy API access.
  flows:
  - authorizationUrl: https://app.quartzy.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.quartzy.com/oauth/token
  name: oauth2
  sources:
  - openapi/quartzy-openapi.yml
  type: oauth2
slug: quartzy-authentication
source_filename: quartzy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quartzy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: Access-Token\n  description: Per-user AccessToken generated in Quartzy under Profile > Access Tokens and sent\n    in the Access-Token header.\n  sources:\n  - openapi/quartzy-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.quartzy.com/oauth/authorize\n    tokenUrl: https://api.quartzy.com/oauth/token\n    scopes: 0\n  description: OAuth2 authorization for Quartzy API access.\n  sources:\n  - openapi/quartzy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/authentication/quartzy-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Lab Management
- Inventory Management
- Life Sciences
- Procurement
- Ordering
- Laboratory
- Webhooks
---
