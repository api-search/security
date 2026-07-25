---
api_key_in: []
api_specs:
- filename: plunk-campaigns-api-openapi.yml
  format: yaml
  label: Plunk Campaigns API
  slug: plunk-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/openapi/plunk-campaigns-api-openapi.yml
- filename: plunk-contacts-api-openapi.yml
  format: yaml
  label: Plunk Contacts API
  slug: plunk-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/openapi/plunk-contacts-api-openapi.yml
- filename: plunk-events-api-openapi.yml
  format: yaml
  label: Plunk Events API
  slug: plunk-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/openapi/plunk-events-api-openapi.yml
- filename: plunk-transactional-api-openapi.yml
  format: yaml
  label: Plunk Transactional API
  slug: plunk-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/openapi/plunk-transactional-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Plunk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plunk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Plunk
provider_slug: plunk
scheme_count: 1
schemes:
- description: Plunk API key passed as a Bearer token. Use a secret key (sk_) for most endpoints; the /track endpoint additionally accepts a public key (pk_).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/plunk-openapi.yml
  type: http
slug: plunk-authentication
source_filename: plunk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/plunk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Plunk API key passed as a Bearer token. Use a secret key (sk_) for most endpoints;\n    the /track endpoint additionally accepts a public key (pk_).\n  sources:\n  - openapi/plunk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/authentication/plunk-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Transactional Email
- Marketing
- Automation
- Open Source
- SaaS
---
