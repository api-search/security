---
anonymous_access: false
api_key_in: []
api_specs:
- filename: drip-apex-com-openapi-generated.yml
  format: yaml
  label: DRIP Apex API
  slug: drip-apex-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drip-apex-com/openapi/_ae-authored/drip-apex-com-openapi-generated.yml
auth_types: []
description: API keys are created per shop as publishable, test secret, or live secret keys and stored hashed. Secret keys are shown once, then used as bearer tokens for /api/v1 requests.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: DRIP Apex Authentication
name_suffix: Authentication
oauth_flows: []
overview: DRIP Apex declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DRIP Apex
provider_slug: drip-apex-com
scheme_count: 1
schemes:
- evidence: Secret keys are shown once, then used as bearer tokens for /api/v1 requests.
  header: Authorization
  how_to_obtain: Create a live or test secret key in the Settings → Developers page; the secret is displayed once and used as a bearer token.
  location: header
  name: API Key
  type: http-bearer
slug: drip-apex-com-authentication
source_filename: drip-apex-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.drip-apex.com/docs/getting-started/access-authentication-workspace-selection
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.drip-apex.com/docs/getting-started/access-authentication-workspace-selection\nsources:\n- https://docs.drip-apex.com/docs/getting-started/access-authentication-workspace-selection\n- https://docs.drip-apex.com/docs/settings-account/api-keys\n- https://docs.drip-apex.com/docs/cli/install-auth\n- https://docs.drip-apex.com/docs/getting-started/what-is-apex\ndescription: API keys are created per shop as publishable, test secret, or live secret keys and stored hashed. Secret keys are shown once, then\n  used as bearer tokens for /api/v1 requests.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Secret keys are shown once, then used as bearer tokens for /api/v1 requests.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a live or test secret key in the Settings → Developers page; the secret is displayed once and used as a bearer token.\nnote:\
  \ No OAuth flows or other authentication schemes are documented on the provided pages.\ndocs: https://docs.drip-apex.com/docs/getting-started/access-authentication-workspace-selection\n"
source_yaml_url: https://artifacts.apis.io/drip-apex-com/authentication/drip-apex-com-authentication.yml
summary_line: 1 scheme
tags:
- A/B Testing
- Artificial Intelligence
- Marketing
- Feature Flags
- Personalization
---
