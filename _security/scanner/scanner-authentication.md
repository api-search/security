---
api_key_in: []
api_specs:
- filename: scanner-ad-hoc-queries-api-openapi.yml
  format: yaml
  label: Scanner Ad Hoc Queries API
  slug: scanner-ad-hoc-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scanner/refs/heads/main/openapi/scanner-ad-hoc-queries-api-openapi.yml
- filename: scanner-detection-rules-api-openapi.yml
  format: yaml
  label: Scanner Detection Rules API
  slug: scanner-detection-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scanner/refs/heads/main/openapi/scanner-detection-rules-api-openapi.yml
- filename: scanner-event-sinks-api-openapi.yml
  format: yaml
  label: Scanner Event Sinks API
  slug: scanner-event-sinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scanner/refs/heads/main/openapi/scanner-event-sinks-api-openapi.yml
- filename: scanner-indexes-api-openapi.yml
  format: yaml
  label: Scanner Indexes API
  slug: scanner-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scanner/refs/heads/main/openapi/scanner-indexes-api-openapi.yml
- filename: scanner-info-api-openapi.yml
  format: yaml
  label: Scanner Info API
  slug: scanner-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scanner/refs/heads/main/openapi/scanner-info-api-openapi.yml
- filename: scanner-lookup-tables-api-openapi.yml
  format: yaml
  label: Scanner Lookup Tables API
  slug: scanner-lookup-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scanner/refs/heads/main/openapi/scanner-lookup-tables-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Scanner Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scanner secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scanner
provider_slug: scanner
scheme_count: 1
schemes:
- description: 'Scanner API key presented as `Authorization: Bearer <Scanner API Key>`. Create keys in Settings > API Keys.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/scanner-openapi.yml
  type: http
slug: scanner-authentication
source_filename: scanner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/scanner-openapi.yml\ndocs: https://docs.scanner.dev/scanner/using-scanner-complete-feature-reference/developer-tools/api\nnotes: >-\n  API access uses a Scanner API key presented as an HTTP Bearer token\n  (Authorization: Bearer <key>); create/manage keys in Settings > API Keys.\n  Console/SSO sign-in is separate, brokered by Stytch, and supports Okta\n  (OIDC/SAML), Google Workspace SAML, Microsoft Entra (OIDC/SAML), most other\n  SAML/OIDC providers, and SCIM provisioning.\nsso:\n  broker: Stytch\n  providers: [Okta OIDC, Okta SAML, Google Workspace SAML, Microsoft Entra OIDC, Microsoft Entra SAML]\n  scim: true\n  docs: https://docs.scanner.dev/scanner/using-scanner-complete-feature-reference/administration/authentication-and-sso\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Scanner API key presented as `Authorization: Bearer <Scanner API Key>`. Create\n\
  \    keys in Settings > API Keys.'\n  sources:\n  - openapi/scanner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scanner/refs/heads/main/authentication/scanner-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- SIEM
- Log Analytics
- Threat Detection
- Security Operations
- Observability
- MCP
---
