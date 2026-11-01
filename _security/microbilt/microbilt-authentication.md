---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microbilt-openapi-generated.yml
  format: yaml
  label: Microbilt API
  slug: microbilt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microbilt/openapi/_ae-authored/microbilt-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Microbilt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microbilt declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Microbilt
provider_slug: microbilt
scheme_count: 1
schemes:
- evidence: Before you can begin the OAuth process, you must first register a new app with the service. After registering your app, you will receive a Client ID and a Client Secret.
  flows:
  - client_credentials
  how_to_obtain: Register a new app to receive a Client ID and a Client Secret.
  name: OAuth2 Client Credentials
  token_url: https://apitest.microbilt.com/OAuth/Token
  type: oauth2
slug: microbilt-authentication
source_filename: microbilt-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.microbilt.com/article/microbilt-apis-oauth-documentation
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.microbilt.com/article/microbilt-apis-oauth-documentation\nsources:\n- https://developer.microbilt.com/article/microbilt-apis-oauth-documentation\n- https://developer.microbilt.com/api-oauth-docs\nschemes:\n- type: oauth2\n  name: OAuth2 Client Credentials\n  evidence: Before you can begin the OAuth process, you must first register a new app with the service. After registering your app, you will receive\n    a Client ID and a Client Secret.\n  flows:\n  - client_credentials\n  token_url: https://apitest.microbilt.com/OAuth/Token\n  how_to_obtain: Register a new app to receive a Client ID and a Client Secret.\ndocs: https://developer.microbilt.com/article/microbilt-apis-oauth-documentation\n"
source_yaml_url: https://artifacts.apis.io/microbilt/authentication/microbilt-authentication.yml
summary_line: 1 scheme
tags:
- Credit Decisioning
- Identity Verification
- Background Screening
- Business Credentialing
- Risk Management
- Alternative Credit Data
- Compliance
---
