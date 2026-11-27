---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hcss-openapi-generated.yml
  format: yaml
  label: Heavy Construction Systems Specialists API
  slug: hcss-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hcss/openapi/_ae-authored/hcss-openapi-generated.yml
auth_types: []
description: HCSS uses OAuth 2.0 client credentials flow. Clients obtain a bearer token from the Identity API and send it in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Heavy Construction Systems Specialists Authentication
name_suffix: Authentication
oauth_flows: []
overview: Heavy Construction Systems Specialists declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Heavy Construction Systems Specialists
provider_slug: hcss
scheme_count: 1
schemes:
- evidence: In most cases, you will use the Client Credentials Flow.
  header: Authorization
  how_to_obtain: A company admin generates a client_id and client_secret via the HCSS credentials webpage (https://hcssapps.com/rs/Clients/Create) and selects the desired scopes.
  location: header
  name: Bearer Token
  token_url: https://api.hcssapps.com/identity/connect/token
  type: http-bearer
slug: hcss-authentication
source_filename: hcss-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.hcssapps.com/hcss/docs/managing-oauth-clients-and-scope-updates.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.hcssapps.com/hcss/docs/managing-oauth-clients-and-scope-updates.md\nsources:\n- https://developer.hcssapps.com/hcss/docs/managing-oauth-clients-and-scope-updates.md\n- https://developer.hcssapps.com/hcss/docs/getting-credentials.md\n- https://developer.hcssapps.com/hcss/docs/request-tokens.md\n- https://developer.hcssapps.com/hcss/docs/client-credentials.md\ndescription: HCSS uses OAuth 2.0 client credentials flow. Clients obtain a bearer token from the Identity API and send it in the Authorization\n  header.\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: In most cases, you will use the Client Credentials Flow.\n  location: header\n  header: Authorization\n  token_url: https://api.hcssapps.com/identity/connect/token\n  how_to_obtain: A company admin generates a client_id and client_secret via the HCSS credentials webpage (https://hcssapps.com/rs/Clients/Create)\n\
  \    and selects the desired scopes.\ndocs: https://developer.hcssapps.com/hcss/docs/managing-oauth-clients-and-scope-updates.md\n"
source_yaml_url: https://artifacts.apis.io/hcss/authentication/hcss-authentication.yml
summary_line: 1 scheme
tags:
- Construction
- Software
- Estimating
- Project Management
- Safety
- Fleet Maintenance
---
