---
api_key_in:
- header
api_specs:
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Campaigns API
  slug: sertifier-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Credentials API
  slug: sertifier-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Designs API
  slug: sertifier-designs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Credential Details API
  slug: sertifier-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Email Templates API
  slug: sertifier-email-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Recipients API
  slug: sertifier-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Attributes API
  slug: sertifier-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Webhooks API
  slug: sertifier-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sertifier Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sertifier secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sertifier
provider_slug: sertifier
scheme_count: 1
schemes:
- description: Private API key obtained from the Sertifier web application under Settings > API & Integrations (also referenced as Advanced > Integrations). Store it in a secrets vault; never embed it in client-side JavaScript.
  in: header
  name: secretKey
  parameter: secretKey
  sources:
  - openapi/sertifier-openapi.yml
  type: apiKey
slug: sertifier-authentication
source_filename: sertifier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sertifier-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: secretKey\n  type: apiKey\n  in: header\n  parameter: secretKey\n  description: Private API key obtained from the Sertifier web application under Settings >\n    API & Integrations (also referenced as Advanced > Integrations). Store it in a secrets vault;\n    never embed it in client-side JavaScript.\n  sources:\n  - openapi/sertifier-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/authentication/sertifier-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Digital Credentials
- Certificates
- Badges
- Open Badges
- Verifiable Credentials
- Credentialing
- EdTech
---
