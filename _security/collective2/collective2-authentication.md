---
anonymous_access: false
api_key_in: []
api_specs:
- filename: collective2-autotrade-api-openapi.yml
  format: yaml
  label: Collective2 Autotrade API
  slug: collective2-autotrade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/collective2/refs/heads/main/openapi/collective2-autotrade-api-openapi.yml
- filename: collective2-general-api-openapi.yml
  format: yaml
  label: Collective2 General API
  slug: collective2-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/collective2/refs/heads/main/openapi/collective2-general-api-openapi.yml
- filename: collective2-strategies-api-openapi.yml
  format: yaml
  label: Collective2 Strategies API
  slug: collective2-strategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/collective2/refs/heads/main/openapi/collective2-strategies-api-openapi.yml
auth_types: []
description: Collective2 API uses an API key passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Collective2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Collective2 declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Collective2
provider_slug: collective2
scheme_count: 1
schemes:
- evidence: Your API key is required to authenticate all API requests.
  header: Authorization
  how_to_obtain: Create an account, log in, and generate an API key in your dashboard.
  location: header
  name: Authorization
  type: apiKey
slug: collective2-authentication
source_filename: collective2-authentication.yml
source_heading: Authentication Profile
source_url: https://api-docs.collective2.com/quickstart.md
source_yaml: "generated: '2026-10-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api-docs.collective2.com/quickstart.md\nsources:\n- https://api-docs.collective2.com/quickstart.md\n- https://api-docs.collective2.com/guides/quickstart.md\ndescription: Collective2 API uses an API key passed as a Bearer token in the Authorization header.\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: Your API key is required to authenticate all API requests.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an account, log in, and generate an API key in your dashboard.\nnote: No OAuth2 flows, JWT, HMAC, MTLS, or other authentication schemes are documented.\ndocs: https://api-docs.collective2.com/quickstart.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collective2/refs/heads/main/authentication/collective2-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Trading
- Marketplace
- Investment
---
