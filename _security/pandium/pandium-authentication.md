---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: pandium-connector-calls-api-openapi.yml
  format: yaml
  label: Pandium Connector Calls API
  slug: pandium-connector-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/openapi/pandium-connector-calls-api-openapi.yml
- filename: pandium-integrations-api-openapi.yml
  format: yaml
  label: Pandium Integrations API
  slug: pandium-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/openapi/pandium-integrations-api-openapi.yml
- filename: pandium-runs-api-openapi.yml
  format: yaml
  label: Pandium Runs API
  slug: pandium-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/openapi/pandium-runs-api-openapi.yml
- filename: pandium-tenant-metadata-api-openapi.yml
  format: yaml
  label: Pandium Tenant Metadata API
  slug: pandium-tenant-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/openapi/pandium-tenant-metadata-api-openapi.yml
- filename: pandium-tenants-api-openapi.yml
  format: yaml
  label: Pandium Tenants API
  slug: pandium-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/openapi/pandium-tenants-api-openapi.yml
- filename: pandium-builds-api-openapi.yml
  format: yaml
  label: Pandium Builds API
  slug: pandium-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/openapi/pandium-builds-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Pandium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pandium secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pandium
provider_slug: pandium
scheme_count: 1
schemes:
- description: 'API key generated in the Pandium Integration Hub: Settings sidebar > API Access tab. Name the key and generate it; keys are only viewable at creation, so they must be stored securely at that moment. Attach the key to every request in the X-API-KEY header.'
  in: header
  name: apiKey
  parameter: X-API-KEY
  sources:
  - https://docs.pandium.com/reference/pandium-api
  - openapi/pandium-tenants-api-openapi.yml
  type: apiKey
slug: pandium-authentication
source_filename: pandium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://docs.pandium.com/reference/pandium-api\ndocs: https://docs.pandium.com/reference/pandium-api\nnote: >-\n  Upgraded 2026-09-03 from the earlier derived profile, which wrongly recorded the key as a\n  Bearer token in the Authorization header. The provider's API reference states the key is\n  attached under an `x-api-key` header. The OpenAPI securitySchemes in openapi/ were corrected to\n  match. Requests without a valid key return 403 {\"detail\": \"Not authorized\"} (observed live,\n  2026-09-03).\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: >-\n    API key generated in the Pandium Integration Hub: Settings sidebar > API Access tab. Name the\n    key and generate it; keys are only viewable at creation, so they must be stored securely at\n    that moment. Attach the key to every request in the X-API-KEY header.\n\
  \  sources:\n  - https://docs.pandium.com/reference/pandium-api\n  - openapi/pandium-tenants-api-openapi.yml\nkey_provisioning:\n  self_serve: true\n  location: Integration Hub > Settings > API Access\n  visibility: only viewable at creation\n  prefix: none documented\noauth: >-\n  The public platform API does not use OAuth. OAuth appears only inside Pandium's managed\n  connector authentication, where the platform holds end-customer credentials for third-party\n  APIs on behalf of tenants.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/authentication/pandium-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- B2B
- Hub
- Integration
- Workflows
- iPaaS
---
