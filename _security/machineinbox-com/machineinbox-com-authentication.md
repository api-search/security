---
anonymous_access: false
api_key_in: []
api_specs:
- filename: machineinbox-com-inboxes-api-openapi.yml
  format: yaml
  label: Machine Inbox Inboxes API
  slug: machineinbox-com-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machineinbox-com/openapi/machineinbox-com-inboxes-api-openapi.yml
- filename: machineinbox-com-messages-api-openapi.yml
  format: yaml
  label: Machine Inbox Messages API
  slug: machineinbox-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machineinbox-com/openapi/machineinbox-com-messages-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Machine Inbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Machine Inbox secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Machine Inbox
provider_slug: machineinbox-com
scheme_count: 1
schemes:
- bearerFormat: MachineInboxToken
  description: 'Use the mi_live_... token returned by inbox creation. The HTTP client adds the Authorization: Bearer prefix.'
  name: mailboxToken
  scheme: bearer
  sources:
  - openapi/machineinbox-com-openapi.json
  type: http
slug: machineinbox-com-authentication
source_filename: machineinbox-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/machineinbox-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: mailboxToken\n  type: http\n  scheme: bearer\n  bearerFormat: MachineInboxToken\n  description: 'Use the mi_live_... token returned by inbox creation. The HTTP client adds the\n    Authorization: Bearer prefix.'\n  sources:\n  - openapi/machineinbox-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/machineinbox-com/authentication/machineinbox-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Artificial Intelligence
- Automation
- Payments
- Services
- Company
---
