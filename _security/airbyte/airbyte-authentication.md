---
api_key_in: []
api_specs:
- filename: airbyte-openapi.yml
  format: yaml
  label: Airbyte
  slug: airbyte
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/openapi/airbyte-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Airbyte Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Airbyte secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Airbyte
provider_slug: airbyte
scheme_count: 1
schemes:
- bearer_format: JWT (RS256)
  description: 'The Airbyte public API authenticates with the OAuth 2.0 client_credentials grant. Create an Application in the Airbyte UI (User settings > Applications) to obtain a client_id and client_secret, then POST them with grant_type=client_credentials to the token endpoint. The returned access token expires after 15 minutes and is sent as an ''Authorization: Bearer <token>'' header. The application represents the creating user and inherits their permissions.'
  flow: clientCredentials
  name: clientCredentials
  scopes:
  - openid
  - api
  token_endpoint_auth_method: client_secret_post
  token_ttl_seconds: 900
  token_url_cloud: https://api.airbyte.com/v1/applications/token
  token_url_self_managed: https://<YOUR_AIRBYTE_URL>/api/public/v1/applications/token
  type: oauth2
slug: airbyte-authentication
source_filename: airbyte-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://docs.airbyte.com/platform/using-airbyte/configuring-api-access\ndocs: https://docs.airbyte.com/platform/using-airbyte/configuring-api-access\ndiscovery: https://airbyte.com/.well-known/openid-configuration\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_delivery: bearer\nschemes:\n- name: clientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url_cloud: https://api.airbyte.com/v1/applications/token\n  token_url_self_managed: https://<YOUR_AIRBYTE_URL>/api/public/v1/applications/token\n  token_endpoint_auth_method: client_secret_post\n  token_ttl_seconds: 900\n  bearer_format: JWT (RS256)\n  scopes: [openid, api]\n  description: >-\n    The Airbyte public API authenticates with the OAuth 2.0 client_credentials\n    grant. Create an Application in the Airbyte UI (User settings > Applications)\n    to obtain a client_id and client_secret, then POST them with\n    grant_type=client_credentials\
  \ to the token endpoint. The returned access\n    token expires after 15 minutes and is sent as an\n    'Authorization: Bearer <token>' header. The application represents the\n    creating user and inherits their permissions.\nnotes: >-\n  The harvested OpenAPI (openapi/airbyte-openapi.yml) declares no\n  securitySchemes, so this profile is captured from the docs and the OIDC\n  discovery document rather than derived. Self-managed/Enterprise deployments\n  additionally support SSO (OIDC/SAML) and RBAC at the platform level.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/authentication/airbyte-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
---
