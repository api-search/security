---
anonymous_access: false
api_key_in: []
api_specs:
- filename: amfionhq-com-fleet-api-openapi.yml
  format: yaml
  label: amfionhq-com Fleet API
  slug: amfionhq-com-fleet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amfionhq-com/openapi/amfionhq-com-fleet-api-openapi.yml
- filename: amfionhq-com-tenants-api-openapi.yml
  format: yaml
  label: amfionhq-com Tenants API
  slug: amfionhq-com-tenants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amfionhq-com/openapi/amfionhq-com-tenants-api-openapi.yml
- filename: amfionhq-com-tools-api-openapi.yml
  format: yaml
  label: amfionhq-com Tools API
  slug: amfionhq-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amfionhq-com/openapi/amfionhq-com-tools-api-openapi.yml
- filename: amfionhq-com-usage-api-openapi.yml
  format: yaml
  label: amfionhq-com Usage API
  slug: amfionhq-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amfionhq-com/openapi/amfionhq-com-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amfionhq Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: amfionhq-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: amfionhq-com
provider_slug: amfionhq-com
scheme_count: 1
schemes:
- bearerFormat: amf_<48 hex chars>
  description: Partner API key. Keys carry scopes; each operation lists its required scope in `x-required-scope`. Suspending a partner blocks all its keys immediately.
  name: partnerKey
  scheme: bearer
  sources:
  - openapi/amfionhq-com-openapi.yml
  type: http
slug: amfionhq-com-authentication
source_filename: amfionhq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/amfionhq-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: partnerKey\n  type: http\n  scheme: bearer\n  bearerFormat: amf_<48 hex chars>\n  description: Partner API key. Keys carry scopes; each operation lists its required scope in\n    `x-required-scope`. Suspending a partner blocks all its keys immediately.\n  sources:\n  - openapi/amfionhq-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amfionhq-com/authentication/amfionhq-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- FrontDesk
- Booking
- Automation
---
