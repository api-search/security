---
api_key_in: []
api_specs:
- filename: buymeacoffee-openapi.yml
  format: yaml
  label: Buy Me a Coffee Supporters API
  slug: buymeacoffee-supporters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buymeacoffee/refs/heads/main/openapi/buymeacoffee-openapi.yml
- filename: buymeacoffee-openapi.yml
  format: yaml
  label: Buy Me a Coffee Subscriptions API
  slug: buymeacoffee-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buymeacoffee/refs/heads/main/openapi/buymeacoffee-openapi.yml
- filename: buymeacoffee-openapi.yml
  format: yaml
  label: Buy Me a Coffee Extras API
  slug: buymeacoffee-extras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buymeacoffee/refs/heads/main/openapi/buymeacoffee-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Buymeacoffee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buy Me a Coffee secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Buy Me a Coffee
provider_slug: buymeacoffee
scheme_count: 1
schemes:
- description: 'Personal access token created in the Buy Me a Coffee Developer Dashboard. Sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/buymeacoffee-openapi.yml
  type: http
slug: buymeacoffee-authentication
source_filename: buymeacoffee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/buymeacoffee-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Personal access token created in the Buy Me a Coffee Developer Dashboard. Sent\n    as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/buymeacoffee-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buymeacoffee/refs/heads/main/authentication/buymeacoffee-authentication.yml
summary_line: http · 1 scheme
tags:
- Creator Economy
- Memberships
- Subscriptions
- Tips
- Payments
- Donations
---
