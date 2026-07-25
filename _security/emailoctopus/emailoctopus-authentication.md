---
api_key_in: []
api_specs:
- filename: emailoctopus-automation-api-openapi.yml
  format: yaml
  label: EmailOctopus Automation API
  slug: emailoctopus-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-automation-api-openapi.yml
- filename: emailoctopus-campaign-api-openapi.yml
  format: yaml
  label: EmailOctopus Campaign API
  slug: emailoctopus-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-campaign-api-openapi.yml
- filename: emailoctopus-contact-api-openapi.yml
  format: yaml
  label: EmailOctopus Contact API
  slug: emailoctopus-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-contact-api-openapi.yml
- filename: emailoctopus-field-api-openapi.yml
  format: yaml
  label: EmailOctopus Field API
  slug: emailoctopus-field-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-field-api-openapi.yml
- filename: emailoctopus-list-api-openapi.yml
  format: yaml
  label: EmailOctopus List API
  slug: emailoctopus-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-list-api-openapi.yml
- filename: emailoctopus-tag-api-openapi.yml
  format: yaml
  label: EmailOctopus Tag API
  slug: emailoctopus-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-tag-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Emailoctopus Authentication
name_suffix: Authentication
oauth_flows: []
overview: EmailOctopus secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EmailOctopus
provider_slug: emailoctopus
scheme_count: 1
schemes:
- description: Bearer API key in the Authorization header. Create a key at https://api.emailoctopus.com/developer/api-keys/create
  name: api_key
  scheme: bearer
  sources:
  - openapi/emailoctopus-openapi.yml
  type: http
slug: emailoctopus-authentication
source_filename: emailoctopus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/emailoctopus-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: api_key\n  type: http\n  scheme: bearer\n  description: Bearer API key in the Authorization header. Create a key at https://api.emailoctopus.com/developer/api-keys/create\n  sources:\n  - openapi/emailoctopus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/authentication/emailoctopus-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Email Marketing
- Newsletters
- Campaigns
- Automation
---
