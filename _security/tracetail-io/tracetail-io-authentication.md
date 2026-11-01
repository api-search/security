---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tracetail-io-identification-api-openapi.yml
  format: yaml
  label: tracetail-io Identification API
  slug: tracetail-io-identification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tracetail-io/openapi/tracetail-io-identification-api-openapi.yml
- filename: tracetail-io-server-api-api-openapi.yml
  format: yaml
  label: tracetail-io Server API
  slug: tracetail-io-server-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tracetail-io/openapi/tracetail-io-server-api-api-openapi.yml
- filename: tracetail-io-service-api-openapi.yml
  format: yaml
  label: tracetail-io Service API
  slug: tracetail-io-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tracetail-io/openapi/tracetail-io-service-api-openapi.yml
- filename: tracetail-io-setup-links-api-openapi.yml
  format: yaml
  label: tracetail-io Setup links API
  slug: tracetail-io-setup-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tracetail-io/openapi/tracetail-io-setup-links-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Tracetail Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: tracetail-io declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: tracetail-io
provider_slug: tracetail-io
scheme_count: 3
schemes:
- description: 'Public API key (`tt_` followed by 64 hex characters). It ships in page HTML and only works from pages on its domain. Also accepted as `Authorization: Bearer`.'
  in: header
  name: X-API-Key
  type: apiKey
- description: 'Secret server key (`tts_` followed by 64 hex characters) from Settings → API keys. Server-side only: requests with an Origin header are refused.'
  scheme: bearer
  type: http
- description: 'The token creating the setup link returned (`tt_setup_` followed by 64 hex characters). Keep it to the agent: it collects the keys.'
  scheme: bearer
  type: http
slug: tracetail-io-authentication
source_filename: tracetail-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://tracetail.io/docs.md\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: \"Public API key (`tt_` followed by 64 hex characters). It ships in page HTML and only works from pages on its domain. Also accepted as `Authorization: Bearer`.\"\n  - type: http\n    scheme: bearer\n    description: \"Secret server key (`tts_` followed by 64 hex characters) from Settings → API keys. Server-side only: requests with an Origin header are refused.\"\n  - type: http\n    scheme: bearer\n    description: \"The token creating the setup link returned (`tt_setup_` followed by 64 hex characters). Keep it to the agent: it collects the keys.\"\n"
source_yaml_url: https://artifacts.apis.io/tracetail-io/authentication/tracetail-io-authentication.yml
summary_line: 3 schemes
tags:
- Browser Fingerprinting
- Privacy
- Analytics
- API
- Device Identification
---
