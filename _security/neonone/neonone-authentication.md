---
api_key_in: []
api_specs:
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Accounts API
  slug: neonone-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Households API
  slug: neonone-households-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Donations API
  slug: neonone-donations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Campaigns API
  slug: neonone-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Memberships API
  slug: neonone-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Events API
  slug: neonone-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Custom Fields API
  slug: neonone-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Orders & Store API
  slug: neonone-orders-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Volunteers API
  slug: neonone-volunteers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
- filename: neonone-openapi.yml
  format: yaml
  label: Neon One Webhooks API
  slug: neonone-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/openapi/neonone-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Neonone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neon One secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Neon One
provider_slug: neonone
scheme_count: 1
schemes:
- description: HTTP Basic Authentication. Username is the Neon CRM organization's Org ID; password is an API key generated for a system user under Settings > User Management.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/neonone-openapi.yml
  type: http
slug: neonone-authentication
source_filename: neonone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/neonone-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication. Username is the Neon CRM organization's Org ID; password\n    is an API key generated for a system user under Settings > User Management.\n  sources:\n  - openapi/neonone-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neonone/refs/heads/main/authentication/neonone-authentication.yml
summary_line: http · 1 scheme
tags:
- Nonprofit
- CRM
- Fundraising
- Donor Management
- Membership Management
- Events
---
