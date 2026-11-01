---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sitegrab-screenshot-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API
  slug: sitegrab-screenshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sitegrab/openapi/sitegrab-screenshot-api-openapi.yml
- filename: sitegrab-checkout-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Checkout API
  slug: sitegrab-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sitegrab/openapi/sitegrab-checkout-api-openapi.yml
- filename: sitegrab-docs-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Docs API
  slug: sitegrab-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sitegrab/openapi/sitegrab-docs-api-openapi.yml
- filename: sitegrab-health-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Health API
  slug: sitegrab-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sitegrab/openapi/sitegrab-health-api-openapi.yml
- filename: sitegrab-keys-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Keys API
  slug: sitegrab-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sitegrab/openapi/sitegrab-keys-api-openapi.yml
- filename: sitegrab-screenshot-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Screenshot API
  slug: sitegrab-screenshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sitegrab/openapi/sitegrab-screenshot-api-openapi.yml
- filename: sitegrab-signup-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Signup API
  slug: sitegrab-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sitegrab/openapi/sitegrab-signup-api-openapi.yml
- filename: sitegrab-sitegrab-screenshot-api-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) SiteGrab Screenshot API
  slug: sitegrab-sitegrab-screenshot-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sitegrab/openapi/sitegrab-sitegrab-screenshot-api-api-openapi.yml
- filename: sitegrab-usage-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Usage API
  slug: sitegrab-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sitegrab/openapi/sitegrab-usage-api-openapi.yml
- filename: sitegrab-webhook-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Webhook API
  slug: sitegrab-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sitegrab/openapi/sitegrab-webhook-api-openapi.yml
auth_types: []
description: Authentication uses an API key passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Sitegrab Authentication
name_suffix: Authentication
oauth_flows: []
overview: SiteGrab Screenshot API (LaminarForge) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SiteGrab Screenshot API (LaminarForge)
provider_slug: sitegrab
scheme_count: 1
schemes:
- evidence: 'Then try it: curl -H ''Authorization: Bearer ***}'' https://api.sitegrab.dev/v1/screenshot?url=https://example.com --output shot.png'
  header: Authorization
  how_to_obtain: 'Generate an API key via POST https://api.sitegrab.dev/v1/keys with a JSON body {"tier": "free"}.'
  location: header
  name: Bearer
  type: http-bearer
slug: sitegrab-authentication
source_filename: sitegrab-authentication.yml
source_heading: Authentication Profile
source_url: https://sitegrab.dev/signup
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://sitegrab.dev/signup\nsources:\n- https://sitegrab.dev/signup\ndescription: Authentication uses an API key passed as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Then try it: curl -H ''Authorization: Bearer ***}'' https://api.sitegrab.dev/v1/screenshot?url=https://example.com --output shot.png'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Generate an API key via POST https://api.sitegrab.dev/v1/keys with a JSON body {\"tier\": \"free\"}.'\ndocs: https://sitegrab.dev/signup\n"
source_yaml_url: https://artifacts.apis.io/sitegrab/authentication/sitegrab-authentication.yml
summary_line: 1 scheme
tags:
- Screenshots
- Automation
- Image
- Web
---
