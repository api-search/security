---
api_key_in: []
api_specs:
- filename: aptean-consumers-api-openapi.yml
  format: yaml
  label: Aptean Consumers API
  slug: aptean-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptean/refs/heads/main/openapi/aptean-consumers-api-openapi.yml
- filename: aptean-eventdefinitions-api-openapi.yml
  format: yaml
  label: Aptean EventDefinitions API
  slug: aptean-eventdefinitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptean/refs/heads/main/openapi/aptean-eventdefinitions-api-openapi.yml
- filename: aptean-events-api-openapi.yml
  format: yaml
  label: Aptean Events API
  slug: aptean-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptean/refs/heads/main/openapi/aptean-events-api-openapi.yml
- filename: aptean-producers-api-openapi.yml
  format: yaml
  label: Aptean Producers API
  slug: aptean-producers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptean/refs/heads/main/openapi/aptean-producers-api-openapi.yml
- filename: aptean-publickeys-api-openapi.yml
  format: yaml
  label: Aptean PublicKeys API
  slug: aptean-publickeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptean/refs/heads/main/openapi/aptean-publickeys-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aptean Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aptean secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aptean
provider_slug: aptean
scheme_count: 1
schemes:
- description: 'JWT Authorization header using the Bearer scheme. Example: "Authorization: Bearer {token}"'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/aptean-integration-platform-openapi-original.json
  type: http
slug: aptean-authentication
source_filename: aptean-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/aptean-integration-platform-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  description: 'JWT Authorization header using the Bearer scheme. Example: \"Authorization: Bearer\n    {token}\"'\n  sources:\n  - openapi/aptean-integration-platform-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aptean/refs/heads/main/authentication/aptean-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Manufacturing
- ERP
- Supply Chain
- Integration
- Event-Driven
- Webhook
- Enterprise Software
---
