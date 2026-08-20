---
api_key_in: []
api_specs:
- filename: loops-so-api-key-api-openapi.yml
  format: yaml
  label: Loops API key API
  slug: loops-so-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-api-key-api-openapi.yml
- filename: loops-so-campaigns-api-openapi.yml
  format: yaml
  label: Loops Campaigns API
  slug: loops-so-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-campaigns-api-openapi.yml
- filename: loops-so-components-api-openapi.yml
  format: yaml
  label: Loops Components API
  slug: loops-so-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-components-api-openapi.yml
- filename: loops-so-contact-properties-api-openapi.yml
  format: yaml
  label: Loops Contact properties API
  slug: loops-so-contact-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-contact-properties-api-openapi.yml
- filename: loops-so-contacts-api-openapi.yml
  format: yaml
  label: Loops Contacts API
  slug: loops-so-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-contacts-api-openapi.yml
- filename: loops-so-dedicated-sending-ips-api-openapi.yml
  format: yaml
  label: Loops Dedicated sending IPs API
  slug: loops-so-dedicated-sending-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-dedicated-sending-ips-api-openapi.yml
- filename: loops-so-email-messages-api-openapi.yml
  format: yaml
  label: Loops Email messages API
  slug: loops-so-email-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-email-messages-api-openapi.yml
- filename: loops-so-events-api-openapi.yml
  format: yaml
  label: Loops Events API
  slug: loops-so-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-events-api-openapi.yml
- filename: loops-so-mailing-lists-api-openapi.yml
  format: yaml
  label: Loops Mailing lists API
  slug: loops-so-mailing-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-mailing-lists-api-openapi.yml
- filename: loops-so-themes-api-openapi.yml
  format: yaml
  label: Loops Themes API
  slug: loops-so-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-themes-api-openapi.yml
- filename: loops-so-transactional-emails-api-openapi.yml
  format: yaml
  label: Loops Transactional emails API
  slug: loops-so-transactional-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-transactional-emails-api-openapi.yml
- filename: loops-so-uploads-api-openapi.yml
  format: yaml
  label: Loops Uploads API
  slug: loops-so-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-uploads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Loops So Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loops secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Loops
provider_slug: loops-so
scheme_count: 1
schemes:
- name: apiKey
  scheme: bearer
  sources:
  - openapi/loops-openapi.yml
  type: http
slug: loops-so-authentication
source_filename: loops-so-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/loops-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/loops-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/authentication/loops-so-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Marketing Email
- Transactional Email
- Email Automation
- Email Campaigns
- Email Workflows
- Contacts
- Audience Management
- Event
- Webhook
- Software-as-a-Service
- Developer Tools
---
