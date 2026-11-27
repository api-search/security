---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sydium-com-openapi-generated.yml
  format: yaml
  label: Sydium API
  slug: sydium-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sydium-com/openapi/_ae-authored/sydium-com-openapi-generated.yml
auth_types: []
description: 'Authenticate with an opaque API key sent as `Authorization: Bearer sk_live_...`.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Sydium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sydium declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Sydium
provider_slug: sydium-com
scheme_count: 1
schemes:
- evidence: 'Authenticate with an opaque API key sent as `Authorization: Bearer sk_live_...`.'
  header: Authorization
  location: header
  name: API Key
  type: http-bearer
slug: sydium-com-authentication
source_filename: sydium-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.sydium.com/authentication
source_yaml: "generated: '2026-11-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.sydium.com/authentication\nsources:\n- https://docs.sydium.com/authentication\n- https://docs.sydium.com/api-reference/liveness-probe-no-auth\n- https://docs.sydium.com/quickstart\ndescription: 'Authenticate with an opaque API key sent as `Authorization: Bearer sk_live_...`.'\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Authenticate with an opaque API key sent as `Authorization: Bearer sk_live_...`.'\n  location: header\n  header: Authorization\ndocs: https://docs.sydium.com/authentication\n"
source_yaml_url: https://artifacts.apis.io/sydium-com/authentication/sydium-com-authentication.yml
summary_line: 1 scheme
tags:
- Social Media
- AI
- SaaS
- Marketing
- Automation
---
