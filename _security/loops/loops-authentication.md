---
api_key_in: []
api_specs:
- filename: loops-api-key-api-openapi.yml
  format: yaml
  label: Loops API key API
  slug: loops-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-api-key-api-openapi.yml
- filename: loops-campaigns-api-openapi.yml
  format: yaml
  label: Loops Campaigns API
  slug: loops-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-campaigns-api-openapi.yml
- filename: loops-components-api-openapi.yml
  format: yaml
  label: Loops Components API
  slug: loops-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-components-api-openapi.yml
- filename: loops-contact-properties-api-openapi.yml
  format: yaml
  label: Loops Contact properties API
  slug: loops-contact-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-contact-properties-api-openapi.yml
- filename: loops-contacts-api-openapi.yml
  format: yaml
  label: Loops Contacts API
  slug: loops-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-contacts-api-openapi.yml
- filename: loops-dedicated-sending-ips-api-openapi.yml
  format: yaml
  label: Loops Dedicated sending IPs API
  slug: loops-dedicated-sending-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-dedicated-sending-ips-api-openapi.yml
- filename: loops-email-messages-api-openapi.yml
  format: yaml
  label: Loops Email messages API
  slug: loops-email-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-email-messages-api-openapi.yml
- filename: loops-events-api-openapi.yml
  format: yaml
  label: Loops Events API
  slug: loops-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-events-api-openapi.yml
- filename: loops-mailing-lists-api-openapi.yml
  format: yaml
  label: Loops Mailing lists API
  slug: loops-mailing-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-mailing-lists-api-openapi.yml
- filename: loops-themes-api-openapi.yml
  format: yaml
  label: Loops Themes API
  slug: loops-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-themes-api-openapi.yml
- filename: loops-transactional-emails-api-openapi.yml
  format: yaml
  label: Loops Transactional emails API
  slug: loops-transactional-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-transactional-emails-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Loops Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loops secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Loops
provider_slug: loops
scheme_count: 1
schemes:
- name: apiKey
  scheme: bearer
  sources:
  - openapi/loops-openapi.yaml
  type: http
slug: loops-authentication
source_filename: loops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/loops-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/loops-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/authentication/loops-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Marketing Automation
- Transactional Email
- SaaS
- Communications
---
