---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chartlink-app-account-api-openapi.yml
  format: yaml
  label: Chartlink Account API
  slug: chartlink-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-account-api-openapi.yml
- filename: chartlink-app-asset-types-api-openapi.yml
  format: yaml
  label: Chartlink Asset Types API
  slug: chartlink-app-asset-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-asset-types-api-openapi.yml
- filename: chartlink-app-assets-api-openapi.yml
  format: yaml
  label: Chartlink Assets API
  slug: chartlink-app-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-assets-api-openapi.yml
- filename: chartlink-app-billing-api-openapi.yml
  format: yaml
  label: Chartlink Billing API
  slug: chartlink-app-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-billing-api-openapi.yml
- filename: chartlink-app-billing-info-api-openapi.yml
  format: yaml
  label: Chartlink Billing Info API
  slug: chartlink-app-billing-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-billing-info-api-openapi.yml
- filename: chartlink-app-brands-api-openapi.yml
  format: yaml
  label: Chartlink Brands API
  slug: chartlink-app-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-brands-api-openapi.yml
- filename: chartlink-app-checkout-link-api-openapi.yml
  format: yaml
  label: Chartlink Checkout Link API
  slug: chartlink-app-checkout-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-checkout-link-api-openapi.yml
- filename: chartlink-app-data-api-openapi.yml
  format: yaml
  label: Chartlink Data API
  slug: chartlink-app-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-data-api-openapi.yml
- filename: chartlink-app-feedback-api-openapi.yml
  format: yaml
  label: Chartlink Feedback API
  slug: chartlink-app-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-feedback-api-openapi.yml
- filename: chartlink-app-fonts-api-openapi.yml
  format: yaml
  label: Chartlink Fonts API
  slug: chartlink-app-fonts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-fonts-api-openapi.yml
- filename: chartlink-app-geographies-api-openapi.yml
  format: yaml
  label: Chartlink Geographies API
  slug: chartlink-app-geographies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-geographies-api-openapi.yml
- filename: chartlink-app-invites-api-openapi.yml
  format: yaml
  label: Chartlink Invites API
  slug: chartlink-app-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-invites-api-openapi.yml
- filename: chartlink-app-keys-api-openapi.yml
  format: yaml
  label: Chartlink Keys API
  slug: chartlink-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-keys-api-openapi.yml
- filename: chartlink-app-oembed-api-openapi.yml
  format: yaml
  label: Chartlink Oembed API
  slug: chartlink-app-oembed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-oembed-api-openapi.yml
- filename: chartlink-app-signup-api-openapi.yml
  format: yaml
  label: Chartlink Signup API
  slug: chartlink-app-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-signup-api-openapi.yml
- filename: chartlink-app-try-api-openapi.yml
  format: yaml
  label: Chartlink Try API
  slug: chartlink-app-try-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-try-api-openapi.yml
- filename: chartlink-app-whoami-api-openapi.yml
  format: yaml
  label: Chartlink Whoami API
  slug: chartlink-app-whoami-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-whoami-api-openapi.yml
- filename: chartlink-app-workspace-api-openapi.yml
  format: yaml
  label: Chartlink Workspace API
  slug: chartlink-app-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-workspace-api-openapi.yml
auth_types: []
description: Authentication schemes for Chartlink API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Chartlink App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chartlink declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Chartlink
provider_slug: chartlink-app
scheme_count: 1
schemes:
- evidence: 'In Claude Code or a script: an API key from their studio (Workspace → API keys for Claude Code and scripts), sent as Authorization: Bearer.'
  header: Authorization
  how_to_obtain: Generate an API key in the studio via Workspace → API keys for Claude Code and scripts.
  location: header
  name: Bearer
  type: http-bearer
slug: chartlink-app-authentication
source_filename: chartlink-app-authentication.yml
source_heading: Authentication Profile
source_url: https://chartlink.app/api/docs#POST/api/signup
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://chartlink.app/api/docs#POST/api/signup\nsources:\n- https://chartlink.app/api/docs#POST/api/signup\n- https://chartlink.app/api/docs#GET/api/keys\n- https://chartlink.app/api/docs#POST/api/keys\n- https://chartlink.app/api/docs#POST/api/account/claim\ndescription: Authentication schemes for Chartlink API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'In Claude Code or a script: an API key from their studio (Workspace → API keys for Claude Code and scripts), sent as Authorization:\n    Bearer.'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the studio via Workspace → API keys for Claude Code and scripts.\ndocs: https://chartlink.app/api/docs#POST/api/signup\n"
source_yaml_url: https://artifacts.apis.io/chartlink-app/authentication/chartlink-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Charts
- Branding
- Artificial Intelligence
- Marketing
- Visualization
---
