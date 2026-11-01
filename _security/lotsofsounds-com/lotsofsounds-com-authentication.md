---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lotsofsounds-com-samples-api-openapi.yml
  format: yaml
  label: lotsofsounds-com Samples API
  slug: lotsofsounds-com-samples-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lotsofsounds-com/openapi/lotsofsounds-com-samples-api-openapi.yml
- filename: lotsofsounds-com-sounds-api-openapi.yml
  format: yaml
  label: lotsofsounds-com Sounds API
  slug: lotsofsounds-com-sounds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lotsofsounds-com/openapi/lotsofsounds-com-sounds-api-openapi.yml
auth_types: []
description: Authentication schemes for lotsofsounds-com
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Lotsofsounds Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: lotsofsounds-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: lotsofsounds-com
provider_slug: lotsofsounds-com
scheme_count: 1
schemes:
- evidence: 'All endpoints (except /api/v1/sounds/sample ) require an API key. Pass it via the x-api-key header:'
  header: x-api-key
  how_to_obtain: API keys are prefixed with los_ and can be created from the API Keys dashboard.
  location: header
  name: API Key
  type: apiKey
slug: lotsofsounds-com-authentication
source_filename: lotsofsounds-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.lotsofsounds.com/docs/getting-started/authentication
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.lotsofsounds.com/docs/getting-started/authentication\nsources:\n- https://www.lotsofsounds.com/docs/getting-started/authentication\n- https://www.lotsofsounds.com/docs/getting-started\ndescription: Authentication schemes for lotsofsounds-com\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'All endpoints (except /api/v1/sounds/sample ) require an API key. Pass it via the x-api-key header:'\n  location: header\n  header: x-api-key\n  how_to_obtain: API keys are prefixed with los_ and can be created from the API Keys dashboard.\nnote: No OAuth2, HTTP Bearer, HTTP Basic, JWT, HMAC, mTLS, or other schemes are documented.\ndocs: https://www.lotsofsounds.com/docs/getting-started/authentication\n"
source_yaml_url: https://artifacts.apis.io/lotsofsounds-com/authentication/lotsofsounds-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Audio
- API
- Free
- CC0
---
