---
api_key_in: []
api_specs:
- filename: urbanfox-customer-api-openapi.yml
  format: yaml
  label: UrbanFox Customer API
  slug: urbanfox-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanfox/refs/heads/main/openapi/urbanfox-customer-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Urbanfox Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: UrbanFox secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: UrbanFox
provider_slug: urbanfox
scheme_count: 1
schemes:
- description: 'OAuth 2.0 client-credentials flow. Request a token from `POST /v2/oauth/token` and send it as `Authorization: Bearer <access_token>`.'
  flows:
  - flow: clientCredentials
    scopes: 13
    tokenUrl: https://api.demo-retail.urbanfox.io/v2/oauth/token
  name: oauth2
  sources:
  - openapi/urbanfox-customer-api-openapi.yml
  type: oauth2
slug: urbanfox-authentication
source_filename: urbanfox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/urbanfox-customer-api-openapi.yml\ndocs: https://docs.urbanfox.io/how-to/authenticate\nnotes: 'Machine-to-machine only: no static API keys. POST /v2/oauth/token follows\n  RFC 6749 client-credentials with an application/x-www-form-urlencoded body\n  (grant_type, client_id, client_secret); the response returns a Bearer JWT with\n  expires_in 86400 (24h). Credentials are per-tenant, and the tenant slug appears\n  in both the API host (api.{tenant_slug}.urbanfox.io) and the request path.\n  Credential rotation is supported without downtime via\n  POST /v2/{tenant_slug}/tenants/rotate-auth-secret\n  (docs: https://docs.urbanfox.io/how-to/rotate-auth-secret). 401 means expired/invalid\n  token (re-authenticate); 403 means missing scope or tenant mismatch.'\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl:\
  \ https://api.demo-retail.urbanfox.io/v2/oauth/token\n    scopes: 13\n  description: 'OAuth 2.0 client-credentials flow. Request a token from `POST /v2/oauth/token`\n    and send it as `Authorization: Bearer <access_token>`.'\n  sources:\n  - openapi/urbanfox-customer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanfox/refs/heads/main/authentication/urbanfox-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fraud Detection
- Payment Fraud
- Account Takeover
- Bot Detection
- Risk Management
- Security
- Artificial Intelligence
- eCommerce
---
