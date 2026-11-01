---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cyrisma-openapi-generated.yml
  format: yaml
  label: CYRISMA API
  slug: cyrisma-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyrisma/openapi/_ae-authored/cyrisma-openapi-generated.yml
auth_types: []
description: Authentication for the Cyrisma New Partner API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cyrisma Authentication
name_suffix: Authentication
oauth_flows: []
overview: CYRISMA declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CYRISMA
provider_slug: cyrisma
scheme_count: 1
schemes:
- evidence: 'The New Partner API authenticates with an **API key**: a client ID and client secret pair. You exchange the pair for a short-lived bearer token, and send that token on every request.'
  header: Authorization
  how_to_obtain: Create an API key in the Cyrisma web platform (Settings → API Keys) to get a client ID and client secret, then exchange them via POST to the token URL.
  location: header
  name: Bearer token
  scopes:
  - pulse.read
  - pulse.write
  token_url: https://ccnnnnnn.cyrisma.com/ta/v1/auth/client-token
  type: http-bearer
slug: cyrisma-authentication
source_filename: cyrisma-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.cyrisma.com/api/partner-api/authentication.md
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.cyrisma.com/api/partner-api/authentication.md\nsources:\n- https://docs.cyrisma.com/api/partner-api/authentication.md\n- https://docs.cyrisma.com/api-reference/auth/exchange-an-api-key-for-an-access-token.md\n- https://docs.cyrisma.com/api-reference/msp-administration/get-a-tenants-authentication-policy.md\n- https://docs.cyrisma.com/api-reference/msp-administration/set-a-tenants-authentication-policy.md\ndescription: Authentication for the Cyrisma New Partner API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'The New Partner API authenticates with an **API key**: a client ID and client secret pair. You exchange the pair for a short-lived\n    bearer token, and send that token on every request.'\n  location: header\n  header: Authorization\n  token_url: https://ccnnnnnn.cyrisma.com/ta/v1/auth/client-token\n  scopes:\n  - pulse.read\n  - pulse.write\n\
  \  how_to_obtain: Create an API key in the Cyrisma web platform (Settings → API Keys) to get a client ID and client secret, then exchange them\n    via POST to the token URL.\ndocs: https://docs.cyrisma.com/api/partner-api/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/cyrisma/authentication/cyrisma-authentication.yml
summary_line: 1 scheme
tags:
- Cybersecurity
- Software-as-a-Service
- Risk Management
- Compliance
- Vulnerability Management
- MSP
---
