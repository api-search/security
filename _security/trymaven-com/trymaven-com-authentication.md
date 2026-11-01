---
anonymous_access: false
api_key_in: []
api_specs:
- filename: trymaven-com-health-api-openapi.yml
  format: yaml
  label: Maven Health API
  slug: trymaven-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymaven-com/openapi/trymaven-com-health-api-openapi.yml
- filename: trymaven-com-public-api-v1-api-openapi.yml
  format: yaml
  label: Maven Public API (v1) API
  slug: trymaven-com-public-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymaven-com/openapi/trymaven-com-public-api-v1-api-openapi.yml
- filename: trymaven-com-retell-api-openapi.yml
  format: yaml
  label: Maven Retell API
  slug: trymaven-com-retell-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymaven-com/openapi/trymaven-com-retell-api-openapi.yml
- filename: trymaven-com-vapi-api-openapi.yml
  format: yaml
  label: Maven VAPI API
  slug: trymaven-com-vapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymaven-com/openapi/trymaven-com-vapi-api-openapi.yml
- filename: trymaven-com-widget-sessions-api-openapi.yml
  format: yaml
  label: Maven Widget Sessions API
  slug: trymaven-com-widget-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymaven-com/openapi/trymaven-com-widget-sessions-api-openapi.yml
auth_types: []
description: 'Maven uses a single authentication scheme: API keys passed as Bearer tokens in the Authorization header.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Trymaven Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maven declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Maven
provider_slug: trymaven-com
scheme_count: 1
schemes:
- evidence: All Maven API requests are authenticated with API keys passed as Bearer tokens.
  header: Authorization
  how_to_obtain: Manage API keys in the Maven Dashboard under Settings > API Keys.
  location: header
  name: API Key
  type: http-bearer
slug: trymaven-com-authentication
source_filename: trymaven-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.trymaven.com/authentication.md
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.trymaven.com/authentication.md\nsources:\n- https://docs.trymaven.com/authentication.md\n- https://docs.trymaven.com/api-reference/public-api-v1/check-auth.md\n- https://docs.trymaven.com/widget/quickstart.md\n- https://docs.trymaven.com/quickstart.md\ndescription: 'Maven uses a single authentication scheme: API keys passed as Bearer tokens in the Authorization header.'\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: All Maven API requests are authenticated with API keys passed as Bearer tokens.\n  location: header\n  header: Authorization\n  how_to_obtain: Manage API keys in the Maven Dashboard under Settings > API Keys.\nnote: No OAuth2 or other authentication methods are documented.\ndocs: https://docs.trymaven.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/trymaven-com/authentication/trymaven-com-authentication.yml
summary_line: 1 scheme
tags:
- Payments
- Voice AI
- Chatbots
- API
- FinTech
- Y-Combinator
---
