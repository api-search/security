---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bugiadata-com-api-openapi.yml
  format: yaml
  label: BugiaData Api API
  slug: bugiadata-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugiadata-com/openapi/_original/bugiadata-com-api-openapi.yml
auth_types: []
description: BugiaData uses an API key for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bugiadata Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: BugiaData declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BugiaData
provider_slug: bugiadata-com
scheme_count: 1
schemes:
- evidence: All protected endpoints require an API key in the X-API-Key header.
  header: X-API-Key
  how_to_obtain: Get your API key after subscribing to a tier (FREE, STARTER, or PRO) via checkout or from your dashboard.
  location: header
  name: X-API-Key
  type: apiKey
slug: bugiadata-com-authentication
source_filename: bugiadata-com-authentication.yml
source_heading: Authentication Profile
source_url: https://bugiadata.com/signup
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://bugiadata.com/signup\nsources:\n- https://bugiadata.com/signup\n- https://bugiadata.com/mcp\n- https://bugiadata.com/docs\ndescription: BugiaData uses an API key for authentication.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: All protected endpoints require an API key in the X-API-Key header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Get your API key after subscribing to a tier (FREE, STARTER, or PRO) via checkout or from your dashboard.\nnote: No OAuth2, HTTP Bearer, HTTP Basic, JWT, HMAC, mTLS, or other schemes are documented.\ndocs: https://bugiadata.com/signup\n"
source_yaml_url: https://artifacts.apis.io/bugiadata-com/authentication/bugiadata-com-authentication.yml
summary_line: 1 scheme
tags:
- Data
- Artificial Intelligence
- Testing
- Fake Data
---
