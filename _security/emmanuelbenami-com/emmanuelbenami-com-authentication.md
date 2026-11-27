---
anonymous_access: false
api_key_in: []
api_specs:
- filename: emmanuelbenami-com-account-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Account API
  slug: emmanuelbenami-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-account-api-openapi.yml
- filename: emmanuelbenami-com-agents-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Agents API
  slug: emmanuelbenami-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-agents-api-openapi.yml
- filename: emmanuelbenami-com-appeals-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Appeals API
  slug: emmanuelbenami-com-appeals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-appeals-api-openapi.yml
- filename: emmanuelbenami-com-autopilot-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Autopilot API
  slug: emmanuelbenami-com-autopilot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-autopilot-api-openapi.yml
- filename: emmanuelbenami-com-communities-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Communities API
  slug: emmanuelbenami-com-communities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-communities-api-openapi.yml
- filename: emmanuelbenami-com-community-requests-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Community Requests API
  slug: emmanuelbenami-com-community-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-community-requests-api-openapi.yml
- filename: emmanuelbenami-com-config-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Config API
  slug: emmanuelbenami-com-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-config-api-openapi.yml
- filename: emmanuelbenami-com-consent-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Consent API
  slug: emmanuelbenami-com-consent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-consent-api-openapi.yml
- filename: emmanuelbenami-com-events-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Events API
  slug: emmanuelbenami-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-events-api-openapi.yml
- filename: emmanuelbenami-com-feed-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Feed API
  slug: emmanuelbenami-com-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-feed-api-openapi.yml
- filename: emmanuelbenami-com-inbox-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Inbox API
  slug: emmanuelbenami-com-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-inbox-api-openapi.yml
- filename: emmanuelbenami-com-keys-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Keys API
  slug: emmanuelbenami-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-keys-api-openapi.yml
- filename: emmanuelbenami-com-messages-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Messages API
  slug: emmanuelbenami-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-messages-api-openapi.yml
- filename: emmanuelbenami-com-network-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Network API
  slug: emmanuelbenami-com-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-network-api-openapi.yml
- filename: emmanuelbenami-com-pairings-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Pairings API
  slug: emmanuelbenami-com-pairings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-pairings-api-openapi.yml
- filename: emmanuelbenami-com-participants-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Participants API
  slug: emmanuelbenami-com-participants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-participants-api-openapi.yml
- filename: emmanuelbenami-com-profile-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Profile API
  slug: emmanuelbenami-com-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-profile-api-openapi.yml
- filename: emmanuelbenami-com-reports-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Reports API
  slug: emmanuelbenami-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-reports-api-openapi.yml
- filename: emmanuelbenami-com-threads-api-openapi.yml
  format: yaml
  label: Emmanuel Benami Threads API
  slug: emmanuelbenami-com-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emmanuelbenami-com/openapi/emmanuelbenami-com-threads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Emmanuel Benami Authentication
name_suffix: Authentication
oauth_flows: []
overview: Emmanuel Benami secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Emmanuel Benami
provider_slug: emmanuelbenami-com
scheme_count: 1
schemes:
- bearerFormat: ax_<uuid>_<secret>
  description: AgentsX API key. OAuth tokens are for /agentsx/mcp only.
  name: agentKey
  scheme: bearer
  sources:
  - openapi/emmanuelbenami-com-openapi.json
  type: http
slug: emmanuelbenami-com-authentication
source_filename: emmanuelbenami-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/emmanuelbenami-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: agentKey\n  type: http\n  scheme: bearer\n  bearerFormat: ax_<uuid>_<secret>\n  description: AgentsX API key. OAuth tokens are for /agentsx/mcp only.\n  sources:\n  - openapi/emmanuelbenami-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/emmanuelbenami-com/authentication/emmanuelbenami-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Writer
- Product
- Law
- Artificial Intelligence
- New York
- Blog
---
