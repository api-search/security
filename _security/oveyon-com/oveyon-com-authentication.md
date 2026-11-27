---
anonymous_access: false
api_key_in: []
api_specs:
- filename: oveyon-com-allow-block-lists-api-openapi.yml
  format: yaml
  label: Oveyon Allow/Block lists API
  slug: oveyon-com-allow-block-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-allow-block-lists-api-openapi.yml
- filename: oveyon-com-domains-api-openapi.yml
  format: yaml
  label: Oveyon Domains API
  slug: oveyon-com-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-domains-api-openapi.yml
- filename: oveyon-com-inbound-api-openapi.yml
  format: yaml
  label: Oveyon Inbound API
  slug: oveyon-com-inbound-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-inbound-api-openapi.yml
- filename: oveyon-com-ip-rules-api-openapi.yml
  format: yaml
  label: Oveyon IP rules API
  slug: oveyon-com-ip-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-ip-rules-api-openapi.yml
- filename: oveyon-com-logs-api-openapi.yml
  format: yaml
  label: Oveyon Logs API
  slug: oveyon-com-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-logs-api-openapi.yml
- filename: oveyon-com-marketing-experimental-api-openapi.yml
  format: yaml
  label: Oveyon Marketing (experimental) API
  slug: oveyon-com-marketing-experimental-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-marketing-experimental-api-openapi.yml
- filename: oveyon-com-messages-api-openapi.yml
  format: yaml
  label: Oveyon Messages API
  slug: oveyon-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-messages-api-openapi.yml
- filename: oveyon-com-meta-api-openapi.yml
  format: yaml
  label: Oveyon Meta API
  slug: oveyon-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-meta-api-openapi.yml
- filename: oveyon-com-nps-csat-surveys-api-openapi.yml
  format: yaml
  label: Oveyon NPS/CSAT surveys API
  slug: oveyon-com-nps-csat-surveys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-nps-csat-surveys-api-openapi.yml
- filename: oveyon-com-send-policies-api-openapi.yml
  format: yaml
  label: Oveyon Send policies API
  slug: oveyon-com-send-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-send-policies-api-openapi.yml
- filename: oveyon-com-sending-api-openapi.yml
  format: yaml
  label: Oveyon Sending API
  slug: oveyon-com-sending-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-sending-api-openapi.yml
- filename: oveyon-com-suppressions-api-openapi.yml
  format: yaml
  label: Oveyon Suppressions API
  slug: oveyon-com-suppressions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-suppressions-api-openapi.yml
- filename: oveyon-com-templates-api-openapi.yml
  format: yaml
  label: Oveyon Templates API
  slug: oveyon-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-templates-api-openapi.yml
- filename: oveyon-com-utilities-api-openapi.yml
  format: yaml
  label: Oveyon Utilities API
  slug: oveyon-com-utilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-utilities-api-openapi.yml
- filename: oveyon-com-webhooks-api-openapi.yml
  format: yaml
  label: Oveyon Webhooks API
  slug: oveyon-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Oveyon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oveyon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oveyon
provider_slug: oveyon-com
scheme_count: 1
schemes:
- description: 'Account API key: `Authorization: Bearer <key>`. Each key carries scopes; the scope an operation requires is in `x-oveyon-scope`.'
  name: bearer
  scheme: bearer
  sources:
  - openapi/oveyon-com-openapi.json
  type: http
slug: oveyon-com-authentication
source_filename: oveyon-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/oveyon-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'Account API key: `Authorization: Bearer <key>`. Each key carries scopes; the\n    scope an operation requires is in `x-oveyon-scope`.'\n  sources:\n  - openapi/oveyon-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/oveyon-com/authentication/oveyon-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Transactional Email
- Email API
- SMTP
- Deliverability
- Audit Trail
- Webhook
- Fintech
- Healthcare
---
