---
anonymous_access: false
api_key_in: []
api_specs:
- filename: laminarforge-dev-format-utils-api-openapi.yml
  format: yaml
  label: LaminarForge API Format Utils API
  slug: laminarforge-dev-format-utils-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laminarforge-dev/openapi/laminarforge-dev-format-utils-api-openapi.yml
- filename: laminarforge-dev-platform-api-openapi.yml
  format: yaml
  label: LaminarForge API Platform API
  slug: laminarforge-dev-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laminarforge-dev/openapi/laminarforge-dev-platform-api-openapi.yml
auth_types: []
description: Authentication schemes as published on the LaminarForge API documentation pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Laminarforge Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: LaminarForge API declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LaminarForge API
provider_slug: laminarforge-dev
scheme_count: 2
schemes:
- evidence: 'curl ''https://lf-text-utils.laminarforge.dev/v1/token-count?text=<text>'' -H ''Authorization: Bearer lf_YourApiKey'''
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
- evidence: '"auth":{"header":"X-API-Key"'
  header: X-API-Key
  location: header
  name: X-API-Key
  type: apiKey
slug: laminarforge-dev-authentication
source_filename: laminarforge-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://laminarforge.dev/docs/text-utils/v1-token-count
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://laminarforge.dev/docs/text-utils/v1-token-count\nsources:\n- https://laminarforge.dev/docs/text-utils/v1-token-count\n- https://laminarforge.dev/docs/security-utils/v1-random-token\n- https://lf-format-utils.laminarforge.dev/v1/register\ndescription: Authentication schemes as published on the LaminarForge API documentation pages.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl ''https://lf-text-utils.laminarforge.dev/v1/token-count?text=<text>'' -H ''Authorization: Bearer lf_YourApiKey'''\n  location: header\n  header: Authorization\n- type: apiKey\n  name: X-API-Key\n  evidence: '\"auth\":{\"header\":\"X-API-Key\"'\n  location: header\n  header: X-API-Key\nnote: 'API keys are obtained by POSTing to the /v1/register endpoint as described in page 3: \"POST this same URL with a JSON body such as {\\\"name\\\":\\\"my-agent\\\",\\\"description\\\":\\\"what\n\
  \  it does\\\"} to receive an API key.\"'\ndocs: https://laminarforge.dev/docs/text-utils/v1-token-count\n"
source_yaml_url: https://artifacts.apis.io/laminarforge-dev/authentication/laminarforge-dev-authentication.yml
summary_line: 2 schemes
tags:
- API Marketplace
- Utilities
- Developer Tools
- Integration
- Cloud Services
---
