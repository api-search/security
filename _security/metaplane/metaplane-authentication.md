---
api_key_in:
- header
api_specs:
- filename: metaplane-api-openapi.yml
  format: yaml
  label: Metaplane API
  slug: metaplane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metaplane/refs/heads/main/openapi/_original/metaplane-api-openapi.yml
- filename: metaplane-connections-api-openapi.yml
  format: yaml
  label: Metaplane Connections API
  slug: metaplane-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metaplane/refs/heads/main/openapi/metaplane-connections-api-openapi.yml
- filename: metaplane-monitors-api-openapi.yml
  format: yaml
  label: Metaplane Monitors API
  slug: metaplane-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metaplane/refs/heads/main/openapi/metaplane-monitors-api-openapi.yml
- filename: metaplane-tags-api-openapi.yml
  format: yaml
  label: Metaplane Tags API
  slug: metaplane-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metaplane/refs/heads/main/openapi/metaplane-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Metaplane Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metaplane secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Metaplane
provider_slug: metaplane
scheme_count: 1
schemes:
- description: Copy in your API key generated from metaplane
  documented_form: 'Authorization: Bearer <YOUR_SECRET_API_TOKEN>'
  in: header
  name: Authorization
  parameter: Authorization
  scopes: []
  sources:
  - openapi/metaplane-connections-api-openapi.yml
  - openapi/metaplane-monitors-api-openapi.yml
  - openapi/metaplane-tags-api-openapi.yml
  - https://docs.metaplane.dev/reference/getting-started
  token_management: https://app.metaplane.dev/account/manage-tokens
  type: apiKey
slug: metaplane-authentication
source_filename: metaplane-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://docs.metaplane.dev/reference/getting-started\nspec_source: openapi/_original/metaplane-api-openapi.yml\ndocs: https://docs.metaplane.dev/reference/getting-started\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid: false\n  mtls: false\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Copy in your API key generated from metaplane\n  documented_form: 'Authorization: Bearer <YOUR_SECRET_API_TOKEN>'\n  token_management: https://app.metaplane.dev/account/manage-tokens\n  scopes: []\n  sources:\n  - openapi/metaplane-connections-api-openapi.yml\n  - openapi/metaplane-monitors-api-openapi.yml\n  - openapi/metaplane-tags-api-openapi.yml\n  - https://docs.metaplane.dev/reference/getting-started\nnotes:\n- >-\n  SPEC/DOCS MISMATCH worth naming. Metaplane's getting-started page states \"This API uses token bearer\n  based authentication\"\
  \ and shows the header as \"Authorization: Bearer <YOUR_SECRET_API_TOKEN>\", but the\n  published OpenAPI models the same thing as an apiKey scheme in the Authorization header with no bearer\n  format. A client generated from the contract alone will send the raw token without the \"Bearer \" prefix.\n  The accurate declaration is type http, scheme bearer.\n- >-\n  Tokens are user-generated at https://app.metaplane.dev/account/manage-tokens and the value is displayed\n  exactly once at creation. No scopes, no expiry and no rotation policy are documented; there is no token\n  or key management operation in the 23-operation public API.\n- >-\n  Probed live 2026-08-29 - GET https://dev.api.metaplane.dev/v1/connections without credentials returns\n  HTTP 401 with an empty text/plain body.\n- >-\n  No OAuth 2.0 and no OIDC. /.well-known/oauth-authorization-server and /.well-known/openid-configuration\n  return 404 on www.metaplane.dev, docs.metaplane.dev and dev.api.metaplane.dev. Enterprise\
  \ SSO\n  (Okta / AD / SAML, per https://www.metaplane.dev/pricing) governs web-app login, not API authorization.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metaplane/refs/heads/main/authentication/metaplane-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AIOps
- Data Observability
- Data Quality
- Anomaly Detection
- Data Lineage
- Monitoring
- Analytics
- Data Engineering
- dbt
- Snowflake
---
