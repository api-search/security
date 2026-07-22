---
api_key_in: []
api_specs:
- filename: sana-openapi.yml
  format: yaml
  label: Sana API
  slug: sana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/openapi/sana-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sana Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Sana secures its APIs with oauth2 and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Sana
provider_slug: sana
scheme_count: 4
schemes:
- credentials:
  - client_id
  - client_secret
  flow: clientCredentials
  grant_type: client_credentials
  name: oauth2ClientCredentials
  note: Create an API client in Sana to obtain client_id/client_secret. GET requests require the `read` scope; POST/PATCH/DELETE require the `write` scope.
  scope_delimiter: comma
  scopes:
  - read
  - write
  sources:
  - https://docs.sana.ai/api-docs/
  token_lifetime_seconds: 3600
  token_type: bearer
  token_url: https://{domain}.sana.ai/api/token
  type: oauth2
- applies_to: all REST endpoints
  header: 'Authorization: Bearer <accessToken>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sana-openapi.yml
  - https://docs.sana.ai/api-docs/
  type: http
- applies_to: xAPI statement submission (/xapi/v1/statements)
  flow: clientCredentials
  name: xapiOauth
  sources:
  - https://docs.sana.ai/api-docs/
  token_url: https://{domain}.sana.ai/api/oauth/token
  type: oauth2
- endpoint: https://{domain}.sana.ai/scim/v2
  name: scim2
  note: SCIM 2.0 user provisioning. Bearer (SCIM token, 1-year validity) for Microsoft Entra/Azure; Basic auth (Client ID / Client Secret) for Okta.
  sources:
  - https://help.sana.ai/en/articles/23062-how-to-configure-scim
  type: bearer-or-basic
  version: '2.0'
slug: sana-authentication
source_filename: sana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sana.ai/api-docs/\ndocs: https://docs.sana.ai/api-docs/\nsummary:\n  types: [oauth2, http]\n  http_schemes: [bearer]\n  oauth2_flows: [clientCredentials]\n  scim: '2.0'\n  sso: [saml2, oidc]\nschemes:\n  - name: oauth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://{domain}.sana.ai/api/token\n    grant_type: client_credentials\n    credentials: [client_id, client_secret]\n    scopes: [read, write]\n    scope_delimiter: comma\n    token_type: bearer\n    token_lifetime_seconds: 3600\n    note: >-\n      Create an API client in Sana to obtain client_id/client_secret. GET requests\n      require the `read` scope; POST/PATCH/DELETE require the `write` scope.\n    sources: [https://docs.sana.ai/api-docs/]\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    applies_to: all REST endpoints\n    header: 'Authorization: Bearer <accessToken>'\n    sources: [openapi/sana-openapi.yml,\
  \ https://docs.sana.ai/api-docs/]\n  - name: xapiOauth\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://{domain}.sana.ai/api/oauth/token\n    applies_to: xAPI statement submission (/xapi/v1/statements)\n    sources: [https://docs.sana.ai/api-docs/]\n  - name: scim2\n    type: bearer-or-basic\n    endpoint: https://{domain}.sana.ai/scim/v2\n    version: '2.0'\n    note: >-\n      SCIM 2.0 user provisioning. Bearer (SCIM token, 1-year validity) for Microsoft\n      Entra/Azure; Basic auth (Client ID / Client Secret) for Okta.\n    sources: [https://help.sana.ai/en/articles/23062-how-to-configure-scim]\nsso:\n  protocols: [SAML 2.0, OIDC]\n  providers: [Okta, Microsoft Entra, OneLogin, JumpCloud, Google Workspace, Auth0, Salesforce, ADFS, Ping Identity, CyberArk]\n  docs: https://help.sana.ai/en/articles/23060-setting-up-sso\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/authentication/sana-authentication.yml
summary_line: oauth2/http · 4 schemes
tags:
- Company
- Enterprise AI
- Artificial Intelligence
- Learning Management
- LMS
- Knowledge Management
- Agents
- SCIM
- xAPI
- REST API
---
