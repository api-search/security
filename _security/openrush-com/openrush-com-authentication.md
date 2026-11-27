---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openrush-com-admin-api-openapi.yml
  format: yaml
  label: OpenRush Admin API
  slug: openrush-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrush-com/openapi/openrush-com-admin-api-openapi.yml
- filename: openrush-com-billing-api-openapi.yml
  format: yaml
  label: OpenRush Billing API
  slug: openrush-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrush-com/openapi/openrush-com-billing-api-openapi.yml
- filename: openrush-com-connections-api-openapi.yml
  format: yaml
  label: OpenRush Connections API
  slug: openrush-com-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrush-com/openapi/openrush-com-connections-api-openapi.yml
- filename: openrush-com-me-api-openapi.yml
  format: yaml
  label: OpenRush Me API
  slug: openrush-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrush-com/openapi/openrush-com-me-api-openapi.yml
- filename: openrush-com-meta-api-openapi.yml
  format: yaml
  label: OpenRush Meta API
  slug: openrush-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrush-com/openapi/openrush-com-meta-api-openapi.yml
- filename: openrush-com-monitoring-api-openapi.yml
  format: yaml
  label: OpenRush Monitoring API
  slug: openrush-com-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrush-com/openapi/openrush-com-monitoring-api-openapi.yml
- filename: openrush-com-team-api-openapi.yml
  format: yaml
  label: OpenRush Team API
  slug: openrush-com-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrush-com/openapi/openrush-com-team-api-openapi.yml
- filename: openrush-com-tools-api-openapi.yml
  format: yaml
  label: OpenRush Tools API
  slug: openrush-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrush-com/openapi/openrush-com-tools-api-openapi.yml
- filename: openrush-com-webhooks-api-openapi.yml
  format: yaml
  label: OpenRush Webhooks API
  slug: openrush-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrush-com/openapi/openrush-com-webhooks-api-openapi.yml
- filename: openrush-com-websites-api-openapi.yml
  format: yaml
  label: OpenRush Websites API
  slug: openrush-com-websites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrush-com/openapi/openrush-com-websites-api-openapi.yml
auth_types: []
description: Authentication methods published on OpenRush documentation
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: OpenRush Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenRush declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: OpenRush
provider_slug: openrush-com
scheme_count: 3
schemes:
- evidence: 'Send your key in the Authorization header: curl "https://api.openrush.com/v1/me/credits" \ -H "Authorization: Bearer $OPENRUSH_KEY "'
  header: Authorization
  how_to_obtain: Create a new key in API access; the full key is returned only once when it is created.
  location: header
  name: API Key (Authorization header, Bearer token)
  type: apiKey
- evidence: 'You can also send: curl "https://api.openrush.com/v1/me/credits" \ -H "X-API-Key: $OPENRUSH_KEY "'
  header: X-API-Key
  how_to_obtain: Create a new key in API access; the full key is returned only once when it is created.
  location: header
  name: API Key (X-API-Key header)
  type: apiKey
- evidence: 'For advanced integrations, public API routes can also accept a valid Dashboard session bearer token: curl "https://api.openrush.com/v1/me/credits" \ -H "Authorization: Bearer $SUPABASE_ACCESS_TOKEN "'
  header: Authorization
  how_to_obtain: Sign in to the OpenRush Dashboard; the session provides a bearer token automatically.
  location: header
  name: Dashboard session bearer token
  type: http-bearer
slug: openrush-com-authentication
source_filename: openrush-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.openrush.com/docs/fundamentals/authentication
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.openrush.com/docs/fundamentals/authentication\nsources:\n- https://www.openrush.com/docs/fundamentals/authentication\n- https://www.openrush.com/docs/quickstart\n- https://www.openrush.com/docs/guides/agent-setup\ndescription: Authentication methods published on OpenRush documentation\nschemes:\n- type: apiKey\n  name: API Key (Authorization header, Bearer token)\n  evidence: 'Send your key in the Authorization header: curl \"https://api.openrush.com/v1/me/credits\" \\ -H \"Authorization: Bearer $OPENRUSH_KEY\n    \"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a new key in API access; the full key is returned only once when it is created.\n- type: apiKey\n  name: API Key (X-API-Key header)\n  evidence: 'You can also send: curl \"https://api.openrush.com/v1/me/credits\" \\ -H \"X-API-Key: $OPENRUSH_KEY \"'\n  location: header\n  header: X-API-Key\n\
  \  how_to_obtain: Create a new key in API access; the full key is returned only once when it is created.\n- type: http-bearer\n  name: Dashboard session bearer token\n  evidence: 'For advanced integrations, public API routes can also accept a valid Dashboard session bearer token: curl \"https://api.openrush.com/v1/me/credits\"\n    \\ -H \"Authorization: Bearer $SUPABASE_ACCESS_TOKEN \"'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in to the OpenRush Dashboard; the session provides a bearer token automatically.\nnote: OpenRush does not publish OAuth flows, token URLs, or scopes in the referenced pages.\ndocs: https://www.openrush.com/docs/fundamentals/authentication\n"
source_yaml_url: https://artifacts.apis.io/openrush-com/authentication/openrush-com-authentication.yml
summary_line: 3 schemes
tags:
- Marketing Intelligence
- SEO
- AI Agents
- Data API
- Competitor Analysis
---
