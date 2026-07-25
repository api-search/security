---
api_key_in:
- header
api_specs:
- filename: mailmodo-campaigns-api-openapi.yml
  format: yaml
  label: Mailmodo Campaigns API
  slug: mailmodo-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-campaigns-api-openapi.yml
- filename: mailmodo-contact-lists-api-openapi.yml
  format: yaml
  label: Mailmodo Contact Lists API
  slug: mailmodo-contact-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-contact-lists-api-openapi.yml
- filename: mailmodo-contacts-api-openapi.yml
  format: yaml
  label: Mailmodo Contacts API
  slug: mailmodo-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-contacts-api-openapi.yml
- filename: mailmodo-events-api-openapi.yml
  format: yaml
  label: Mailmodo Events API
  slug: mailmodo-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-events-api-openapi.yml
- filename: mailmodo-templates-api-openapi.yml
  format: yaml
  label: Mailmodo Templates API
  slug: mailmodo-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-templates-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mailmodo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailmodo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mailmodo
provider_slug: mailmodo
scheme_count: 1
schemes:
- description: API key issued from the Mailmodo dashboard at https://manage.mailmodo.com/app/settings/apikey. Sent as the `mmApiKey` request header on every call.
  in: header
  name: ApiKeyAuth
  parameter: mmApiKey
  sources:
  - openapi/mailmodo-openapi.yml
  type: apiKey
slug: mailmodo-authentication
source_filename: mailmodo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mailmodo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: mmApiKey\n  description: API key issued from the Mailmodo dashboard at https://manage.mailmodo.com/app/settings/apikey.\n    Sent as the `mmApiKey` request header on every call.\n  sources:\n  - openapi/mailmodo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/authentication/mailmodo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Email
- Interactive Email
- AMP for Email
- Marketing Automation
- Transactional Email
- Campaigns
- Journeys
- Customer Engagement
---
