---
anonymous_access: false
api_key_in: []
api_specs:
- filename: codeqr-io-analytics-api-openapi.yml
  format: yaml
  label: CodeQR Analytics API
  slug: codeqr-io-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-analytics-api-openapi.yml
- filename: codeqr-io-domains-api-openapi.yml
  format: yaml
  label: CodeQR Domains API
  slug: codeqr-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-domains-api-openapi.yml
- filename: codeqr-io-events-api-openapi.yml
  format: yaml
  label: CodeQR Events API
  slug: codeqr-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-events-api-openapi.yml
- filename: codeqr-io-folders-api-openapi.yml
  format: yaml
  label: CodeQR Folders API
  slug: codeqr-io-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-folders-api-openapi.yml
- filename: codeqr-io-links-api-openapi.yml
  format: yaml
  label: CodeQR Links API
  slug: codeqr-io-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-links-api-openapi.yml
- filename: codeqr-io-projects-api-openapi.yml
  format: yaml
  label: CodeQR Projects API
  slug: codeqr-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-projects-api-openapi.yml
- filename: codeqr-io-qr-codes-api-openapi.yml
  format: yaml
  label: CodeQR QR Codes API
  slug: codeqr-io-qr-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-qr-codes-api-openapi.yml
- filename: codeqr-io-tags-api-openapi.yml
  format: yaml
  label: CodeQR Tags API
  slug: codeqr-io-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-tags-api-openapi.yml
- filename: codeqr-io-track-api-openapi.yml
  format: yaml
  label: CodeQR Track API
  slug: codeqr-io-track-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-track-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CodeQR Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodeQR declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CodeQR
provider_slug: codeqr-io
scheme_count: 2
schemes:
- description: Project-scoped API key; permissions All / Read only / Restricted; can be tied to a user or a machine user.
  format: 'Authorization: Bearer codeqr_xxxxxx'
  from_spec: true
  header: Authorization
  in: header
  key_prefix: codeqr_
  name: token
  scheme: bearer
  type: http
- description: Documented for third-party integrations; not declared in the OpenAPI securitySchemes.
  flows:
    authorizationCode:
      authorizationUrl: https://app.codeqr.io/oauth/authorize
      pkce: recommended for native/SPA clients
      refresh: true
      tokenUrl: https://api.codeqr.io/oauth/token
  from_spec: false
  name: oauth2
  token_lifetime: default expires_in 604,800 seconds (7 days)
  type: oauth2
slug: codeqr-io-authentication
source_filename: codeqr-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.codeqr.io/api-reference/introduction.md\ndocs: https://docs.codeqr.io/api-reference/tokens.md\nschemes:\n- name: token\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer codeqr_xxxxxx'\n  key_prefix: codeqr_\n  description: Project-scoped API key; permissions All / Read only / Restricted; can be tied to a user or a machine user.\n  from_spec: true\n- name: oauth2\n  type: oauth2\n  from_spec: false\n  flows:\n    authorizationCode:\n      authorizationUrl: https://app.codeqr.io/oauth/authorize\n      tokenUrl: https://api.codeqr.io/oauth/token\n      refresh: true\n      pkce: recommended for native/SPA clients\n  token_lifetime: default expires_in 604,800 seconds (7 days)\n  description: Documented for third-party integrations; not declared in the OpenAPI securitySchemes.\nnote: OAuth endpoints read from docs only; not called.\ndocs_additional:\n- https://docs.codeqr.io/integrations/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/codeqr-io/authentication/codeqr-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- QR Codes
- Short Links
- URL Shorteners
- Link Management
- Analytics
- Marketing
- MCP
---
