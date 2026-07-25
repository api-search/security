---
api_key_in: []
api_specs:
- filename: insightly-contacts-api-openapi.yml
  format: yaml
  label: Insightly Contacts API
  slug: insightly-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insightly/refs/heads/main/openapi/insightly-contacts-api-openapi.yml
- filename: insightly-leads-api-openapi.yml
  format: yaml
  label: Insightly Leads API
  slug: insightly-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insightly/refs/heads/main/openapi/insightly-leads-api-openapi.yml
- filename: insightly-opportunities-api-openapi.yml
  format: yaml
  label: Insightly Opportunities API
  slug: insightly-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insightly/refs/heads/main/openapi/insightly-opportunities-api-openapi.yml
- filename: insightly-organisations-api-openapi.yml
  format: yaml
  label: Insightly Organisations API
  slug: insightly-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insightly/refs/heads/main/openapi/insightly-organisations-api-openapi.yml
- filename: insightly-products-api-openapi.yml
  format: yaml
  label: Insightly Products API
  slug: insightly-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insightly/refs/heads/main/openapi/insightly-products-api-openapi.yml
- filename: insightly-projects-api-openapi.yml
  format: yaml
  label: Insightly Projects API
  slug: insightly-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insightly/refs/heads/main/openapi/insightly-projects-api-openapi.yml
- filename: insightly-quotations-api-openapi.yml
  format: yaml
  label: Insightly Quotations API
  slug: insightly-quotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insightly/refs/heads/main/openapi/insightly-quotations-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Insightly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Insightly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Insightly
provider_slug: insightly
scheme_count: 1
schemes:
- description: 'Username is the Base64-encoded API key; password is left blank.

    Example header: Authorization: Basic <base64(apiKey:)>'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/insightly-openapi.yml
  type: http
slug: insightly-authentication
source_filename: insightly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/insightly-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Username is the Base64-encoded API key; password is left blank.\n    Example header: Authorization: Basic <base64(apiKey:)>\n  sources:\n  - openapi/insightly-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insightly/refs/heads/main/authentication/insightly-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Project Management
- Lead Management
- Opportunities
- Contacts
- SMB
---
