---
api_key_in:
- header
api_specs:
- filename: getresponse-accounts-api-openapi.yml
  format: yaml
  label: GetResponse Accounts API
  slug: getresponse-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getresponse/refs/heads/main/openapi/getresponse-accounts-api-openapi.yml
- filename: getresponse-autoresponders-api-openapi.yml
  format: yaml
  label: GetResponse Autoresponders API
  slug: getresponse-autoresponders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getresponse/refs/heads/main/openapi/getresponse-autoresponders-api-openapi.yml
- filename: getresponse-campaigns-api-openapi.yml
  format: yaml
  label: GetResponse Campaigns API
  slug: getresponse-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getresponse/refs/heads/main/openapi/getresponse-campaigns-api-openapi.yml
- filename: getresponse-contacts-api-openapi.yml
  format: yaml
  label: GetResponse Contacts API
  slug: getresponse-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getresponse/refs/heads/main/openapi/getresponse-contacts-api-openapi.yml
- filename: getresponse-custom-fields-api-openapi.yml
  format: yaml
  label: GetResponse Custom Fields API
  slug: getresponse-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getresponse/refs/heads/main/openapi/getresponse-custom-fields-api-openapi.yml
- filename: getresponse-newsletters-api-openapi.yml
  format: yaml
  label: GetResponse Newsletters API
  slug: getresponse-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getresponse/refs/heads/main/openapi/getresponse-newsletters-api-openapi.yml
- filename: getresponse-tags-api-openapi.yml
  format: yaml
  label: GetResponse Tags API
  slug: getresponse-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getresponse/refs/heads/main/openapi/getresponse-tags-api-openapi.yml
- filename: getresponse-webhooks-api-openapi.yml
  format: yaml
  label: GetResponse Webhooks API
  slug: getresponse-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getresponse/refs/heads/main/openapi/getresponse-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Getresponse Authentication
name_suffix: Authentication
oauth_flows: []
overview: GetResponse secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GetResponse
provider_slug: getresponse
scheme_count: 1
schemes:
- description: 'Personal API key sent as "api-key YOUR_API_KEY". Keys expire after 90

    days of inactivity.'
  in: header
  name: apiKey
  parameter: X-Auth-Token
  sources:
  - openapi/getresponse-openapi.yml
  type: apiKey
slug: getresponse-authentication
source_filename: getresponse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/getresponse-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: |-\n    Personal API key sent as \"api-key YOUR_API_KEY\". Keys expire after 90\n    days of inactivity.\n  sources:\n  - openapi/getresponse-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getresponse/refs/heads/main/authentication/getresponse-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Email Marketing
- Marketing Automation
- Landing Pages
- Webinars
- Conversion Funnels
- CRM
---
