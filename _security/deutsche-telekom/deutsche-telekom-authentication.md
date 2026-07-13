---
api_key_in: []
api_specs:
- filename: controlplane-rover-server-openapi.yml
  format: yaml
  label: TARDIS Rover API
  slug: tardis-rover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-rover-server-openapi.yml
- filename: controlplane-cpapi-openapi.yml
  format: yaml
  label: TARDIS Controlplane API
  slug: tardis-controlplane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-cpapi-openapi.yml
- filename: controlplane-identity-openapi.yml
  format: yaml
  label: TARDIS Identity API
  slug: tardis-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-identity-openapi.yml
- filename: controlplane-discovery-application-openapi.yml
  format: yaml
  label: TARDIS Discovery Application API
  slug: tardis-discovery-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-discovery-application-openapi.yml
- filename: controlplane-discovery-event-openapi.yml
  format: yaml
  label: TARDIS Discovery Event API
  slug: tardis-discovery-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-discovery-event-openapi.yml
- filename: controlplane-discovery-stargate-openapi.yml
  format: yaml
  label: TARDIS Discovery Stargate API
  slug: tardis-discovery-stargate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-discovery-stargate-openapi.yml
- filename: controlplane-file-manager-openapi.yml
  format: yaml
  label: TARDIS File Manager API
  slug: tardis-file-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-file-manager-openapi.yml
- filename: controlplane-secret-manager-openapi.yml
  format: yaml
  label: TARDIS Secret Manager API
  slug: tardis-secret-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/openapi/controlplane-secret-manager-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Deutsche Telekom Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Deutsche Telekom secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Deutsche Telekom
provider_slug: deutsche-telekom
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT Bearer token authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/controlplane-file-manager-openapi.yml
  - openapi/controlplane-identity-openapi.yml
  type: http
- description: OAuth2 client_credentials flow
  flows:
  - flow: clientCredentials
    scopes: 13
    tokenUrl: https://example.com/auth/realms/realm//protocol/openid-connect/token
  name: OAuth2
  sources:
  - openapi/controlplane-rover-server-openapi.yml
  type: oauth2
slug: deutsche-telekom-authentication
source_filename: deutsche-telekom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/controlplane-file-manager-openapi.yml, openapi/controlplane-identity-openapi.yml,\n  openapi/controlplane-rover-server-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT Bearer token authentication\n  sources:\n  - openapi/controlplane-file-manager-openapi.yml\n  - openapi/controlplane-identity-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/auth/realms/realm//protocol/openid-connect/token\n    scopes: 13\n  description: OAuth2 client_credentials flow\n  sources:\n  - openapi/controlplane-rover-server-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/authentication/deutsche-telekom-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Telecommunications
- Telco
- Mobile Network Operator
- CPaaS
- Network API
- 5G
- Cloud
- Identity
- Number Verification
- Open Gateway
- CAMARA
- T-Systems
- T-Mobile
- Magenta
- MagentaBusiness
- API Gateway
- Open Source
- Germany
- Europe
---
