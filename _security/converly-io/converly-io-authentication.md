---
anonymous_access: false
api_key_in: []
api_specs:
- filename: converly-io-action-types-api-openapi.yml
  format: yaml
  label: Converly Action Types API
  slug: converly-io-action-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-action-types-api-openapi.yml
- filename: converly-io-billing-api-openapi.yml
  format: yaml
  label: Converly Billing API
  slug: converly-io-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-billing-api-openapi.yml
- filename: converly-io-destination-types-api-openapi.yml
  format: yaml
  label: Converly Destination Types API
  slug: converly-io-destination-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-destination-types-api-openapi.yml
- filename: converly-io-destinations-api-openapi.yml
  format: yaml
  label: Converly Destinations API
  slug: converly-io-destinations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-destinations-api-openapi.yml
- filename: converly-io-events-api-openapi.yml
  format: yaml
  label: Converly Events API
  slug: converly-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-events-api-openapi.yml
- filename: converly-io-flows-api-openapi.yml
  format: yaml
  label: Converly Flows API
  slug: converly-io-flows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-flows-api-openapi.yml
- filename: converly-io-handoffs-api-openapi.yml
  format: yaml
  label: Converly Handoffs API
  slug: converly-io-handoffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-handoffs-api-openapi.yml
- filename: converly-io-invoices-api-openapi.yml
  format: yaml
  label: Converly Invoices API
  slug: converly-io-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-invoices-api-openapi.yml
- filename: converly-io-plans-api-openapi.yml
  format: yaml
  label: Converly Plans API
  slug: converly-io-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-plans-api-openapi.yml
- filename: converly-io-signup-api-openapi.yml
  format: yaml
  label: Converly Signup API
  slug: converly-io-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-signup-api-openapi.yml
- filename: converly-io-site-integrations-api-openapi.yml
  format: yaml
  label: Converly Site Integrations API
  slug: converly-io-site-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-site-integrations-api-openapi.yml
- filename: converly-io-sites-api-openapi.yml
  format: yaml
  label: Converly Sites API
  slug: converly-io-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-sites-api-openapi.yml
- filename: converly-io-subscription-api-openapi.yml
  format: yaml
  label: Converly Subscription API
  slug: converly-io-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-subscription-api-openapi.yml
- filename: converly-io-test-event-api-openapi.yml
  format: yaml
  label: Converly Test Event API
  slug: converly-io-test-event-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-test-event-api-openapi.yml
- filename: converly-io-trigger-types-api-openapi.yml
  format: yaml
  label: Converly Trigger Types API
  slug: converly-io-trigger-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-trigger-types-api-openapi.yml
- filename: converly-io-usage-api-openapi.yml
  format: yaml
  label: Converly Usage API
  slug: converly-io-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converly-io/openapi/converly-io-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Converly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Converly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Converly
provider_slug: converly-io
scheme_count: 1
schemes:
- bearerFormat: sk_live_...
  description: Converly uses API keys. Send your key as a bearer token on every request. There are no OAuth flows for the REST API itself.
  header: 'Authorization: Bearer sk_live_…'
  in: header
  key_prefix: sk_live_
  name: BearerAuth
  provisioning: API access is available on request while the program is in early access. Contact help@converly.io and we'll issue you a key.
  rotation: If a key leaks, ask us to revoke it and issue a new one. Revoking takes effect immediately.
  scheme: bearer
  sources:
  - openapi/converly-io-openapi.yml
  test_keys: There is no separate test key.
  type: http
slug: converly-io-authentication
source_filename: converly-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://developers.converly.io/authentication\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: sk_live_...\n  sources:\n  - openapi/converly-io-openapi.yml\n  in: header\n  header: 'Authorization: Bearer sk_live_…'\n  key_prefix: sk_live_\n  description: Converly uses API keys. Send your key as a bearer token on every request. There are no OAuth flows for the\n    REST API itself.\n  provisioning: API access is available on request while the program is in early access. Contact help@converly.io and we'll\n    issue you a key.\n  test_keys: There is no separate test key.\n  rotation: If a key leaks, ask us to revoke it and issue a new one. Revoking takes effect immediately.\ndocs: https://developers.converly.io/authentication\npermissions:\n  note: 'Keys carry the permissions of their account; a valid key lacking a permission returns 403 insufficient_scope. Permission\n\
  \    names the docs mention (no complete list is published):'\n  named:\n  - account:read\n  - billing:write\n  - billing:cancel\n  - destinations:disconnect\n  - flows:read\n  source: https://developers.converly.io/account\nother_surfaces:\n- surface: MCP server\n  endpoint: https://app.converly.io/mcp\n  auth: OAuth authorization when adding the connector (Claude/ChatGPT)\n  docs: https://developers.converly.io/mcp\n- surface: CLI\n  auth: converly login browser flow storing a credential in ~/.converly/config.json, or CONVERLY_API_KEY env var for headless\n    use\n  docs: https://developers.converly.io/cli\nnotes: The spec also declares an InternalBearer scheme (shared internal secret) used by /v1/signup and internal job endpoints;\n  it is not a customer credential.\n"
source_yaml_url: https://artifacts.apis.io/converly-io/authentication/converly-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Conversion Tracking
- Marketing
- Advertising
- Analytics
- MCP
- REST API
---
