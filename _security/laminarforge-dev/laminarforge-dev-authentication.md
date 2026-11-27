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
- filename: laminarforge-dev-agent-tools-api-openapi.yml
  format: yaml
  label: LaminarForge API Agent Tools API
  slug: laminarforge-dev-agent-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laminarforge-dev/openapi/laminarforge-dev-agent-tools-api-openapi.yml
- filename: laminarforge-dev-business-utils-api-openapi.yml
  format: yaml
  label: LaminarForge API Business Utils API
  slug: laminarforge-dev-business-utils-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laminarforge-dev/openapi/laminarforge-dev-business-utils-api-openapi.yml
- filename: laminarforge-dev-image-utils-api-openapi.yml
  format: yaml
  label: LaminarForge API Image Utils API
  slug: laminarforge-dev-image-utils-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laminarforge-dev/openapi/laminarforge-dev-image-utils-api-openapi.yml
- filename: laminarforge-dev-pricing-api-openapi.yml
  format: yaml
  label: LaminarForge API Pricing API
  slug: laminarforge-dev-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laminarforge-dev/openapi/laminarforge-dev-pricing-api-openapi.yml
- filename: laminarforge-dev-security-utils-api-openapi.yml
  format: yaml
  label: LaminarForge API Security Utils API
  slug: laminarforge-dev-security-utils-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laminarforge-dev/openapi/laminarforge-dev-security-utils-api-openapi.yml
- filename: laminarforge-dev-text-utils-api-openapi.yml
  format: yaml
  label: LaminarForge API Text Utils API
  slug: laminarforge-dev-text-utils-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laminarforge-dev/openapi/laminarforge-dev-text-utils-api-openapi.yml
- filename: laminarforge-dev-validation-utils-api-openapi.yml
  format: yaml
  label: LaminarForge API Validation Utils API
  slug: laminarforge-dev-validation-utils-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laminarforge-dev/openapi/laminarforge-dev-validation-utils-api-openapi.yml
- filename: laminarforge-dev-vps-browser-api-openapi.yml
  format: yaml
  label: LaminarForge API VPS Browser API
  slug: laminarforge-dev-vps-browser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laminarforge-dev/openapi/laminarforge-dev-vps-browser-api-openapi.yml
- filename: laminarforge-dev-web-intel-api-openapi.yml
  format: yaml
  label: LaminarForge API Web Intel API
  slug: laminarforge-dev-web-intel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laminarforge-dev/openapi/laminarforge-dev-web-intel-api-openapi.yml
auth_types: []
description: Authentication schemes as published on LaminarForge API documentation pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LaminarForge API Authentication
name_suffix: Authentication
oauth_flows: []
overview: LaminarForge API declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LaminarForge API
provider_slug: laminarforge-dev
scheme_count: 2
schemes:
- evidence: '-H ''Authorization: Bearer lf_YourApiKey'''
  header: Authorization
  how_to_obtain: Use your API key prefixed with "Bearer " in the Authorization header.
  location: header
  name: Bearer
  type: http-bearer
- evidence: '"header":"X-API-Key"'
  header: X-API-Key
  how_to_obtain: Provide the API key in the X-API-Key header.
  location: header
  name: X-API-Key
  type: apiKey
slug: laminarforge-dev-authentication
source_filename: laminarforge-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://laminarforge.dev/docs/text-utils/v1-token-count
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://laminarforge.dev/docs/text-utils/v1-token-count\nsources:\n- https://laminarforge.dev/docs/text-utils/v1-token-count\n- https://laminarforge.dev/docs/security-utils/v1-random-token\n- https://lf-format-utils.laminarforge.dev/v1/register\ndescription: Authentication schemes as published on LaminarForge API documentation pages.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '-H ''Authorization: Bearer lf_YourApiKey'''\n  location: header\n  header: Authorization\n  how_to_obtain: Use your API key prefixed with \"Bearer \" in the Authorization header.\n- type: apiKey\n  name: X-API-Key\n  evidence: '\"header\":\"X-API-Key\"'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Provide the API key in the X-API-Key header.\ndocs: https://laminarforge.dev/docs/text-utils/v1-token-count\n"
source_yaml_url: https://artifacts.apis.io/laminarforge-dev/authentication/laminarforge-dev-authentication.yml
summary_line: 2 schemes
tags:
- API Marketplace
- Utilities
- Developer Tools
- Integration
- Cloud Services
---
