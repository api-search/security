---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mentio-dev-alerts-api-openapi.yml
  format: yaml
  label: mentio-dev Alerts API
  slug: mentio-dev-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-alerts-api-openapi.yml
- filename: mentio-dev-analytics-api-openapi.yml
  format: yaml
  label: mentio-dev Analytics API
  slug: mentio-dev-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-analytics-api-openapi.yml
- filename: mentio-dev-api-keys-api-openapi.yml
  format: yaml
  label: mentio-dev API keys API
  slug: mentio-dev-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-api-keys-api-openapi.yml
- filename: mentio-dev-attention-api-openapi.yml
  format: yaml
  label: mentio-dev Attention API
  slug: mentio-dev-attention-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-attention-api-openapi.yml
- filename: mentio-dev-auth-api-openapi.yml
  format: yaml
  label: mentio-dev Auth API
  slug: mentio-dev-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-auth-api-openapi.yml
- filename: mentio-dev-billing-api-openapi.yml
  format: yaml
  label: mentio-dev Billing API
  slug: mentio-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-billing-api-openapi.yml
- filename: mentio-dev-company-api-openapi.yml
  format: yaml
  label: mentio-dev Company API
  slug: mentio-dev-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-company-api-openapi.yml
- filename: mentio-dev-feeds-api-openapi.yml
  format: yaml
  label: mentio-dev Feeds API
  slug: mentio-dev-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-feeds-api-openapi.yml
- filename: mentio-dev-filters-api-openapi.yml
  format: yaml
  label: mentio-dev Filters API
  slug: mentio-dev-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-filters-api-openapi.yml
- filename: mentio-dev-groups-api-openapi.yml
  format: yaml
  label: mentio-dev Groups API
  slug: mentio-dev-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-groups-api-openapi.yml
- filename: mentio-dev-keywords-api-openapi.yml
  format: yaml
  label: mentio-dev Keywords API
  slug: mentio-dev-keywords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-keywords-api-openapi.yml
- filename: mentio-dev-members-api-openapi.yml
  format: yaml
  label: mentio-dev Members API
  slug: mentio-dev-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-members-api-openapi.yml
- filename: mentio-dev-mentions-api-openapi.yml
  format: yaml
  label: mentio-dev Mentions API
  slug: mentio-dev-mentions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-mentions-api-openapi.yml
- filename: mentio-dev-people-api-openapi.yml
  format: yaml
  label: mentio-dev People API
  slug: mentio-dev-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-people-api-openapi.yml
- filename: mentio-dev-segments-api-openapi.yml
  format: yaml
  label: mentio-dev Segments API
  slug: mentio-dev-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-segments-api-openapi.yml
- filename: mentio-dev-system-api-openapi.yml
  format: yaml
  label: mentio-dev System API
  slug: mentio-dev-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-system-api-openapi.yml
- filename: mentio-dev-usage-api-openapi.yml
  format: yaml
  label: mentio-dev Usage API
  slug: mentio-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-usage-api-openapi.yml
- filename: mentio-dev-views-api-openapi.yml
  format: yaml
  label: mentio-dev Views API
  slug: mentio-dev-views-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentio-dev/openapi/mentio-dev-views-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mentio Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: mentio-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: mentio-dev
provider_slug: mentio-dev
scheme_count: 1
schemes:
- evidence: 'Every request to the API (and to the [MCP server](/mcp)) is authenticated with a Bearer API key scoped to your workspace:'
  header: Authorization
  how_to_obtain: Create a key via POST /v1/api-keys (see Managing keys table).
  location: header
  name: Bearer
  type: http-bearer
slug: mentio-dev-authentication
source_filename: mentio-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.mentio.dev/authentication.mdx
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.mentio.dev/authentication.mdx\nsources:\n- https://docs.mentio.dev/authentication.mdx\n- https://docs.mentio.dev/api/api-keys/create-api-key.mdx\n- https://docs.mentio.dev/api/api-keys/list-api-keys.mdx\n- https://docs.mentio.dev/api/api-keys/revoke-api-key.mdx\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request to the API (and to the [MCP server](/mcp)) is authenticated with a Bearer API key scoped to your workspace:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key via POST /v1/api-keys (see Managing keys table).\ndocs: https://docs.mentio.dev/authentication.mdx\n"
source_yaml_url: https://artifacts.apis.io/mentio-dev/authentication/mentio-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Social Listening
- AI Integration
- SDKs
- Real-time Monitoring
---
