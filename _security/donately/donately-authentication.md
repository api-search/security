---
api_key_in: []
api_specs:
- filename: donately-openapi.yml
  format: yaml
  label: Donately Donations API
  slug: donately-donations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donately/refs/heads/main/openapi/donately-openapi.yml
- filename: donately-openapi.yml
  format: yaml
  label: Donately People API
  slug: donately-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donately/refs/heads/main/openapi/donately-openapi.yml
- filename: donately-openapi.yml
  format: yaml
  label: Donately Campaigns API
  slug: donately-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donately/refs/heads/main/openapi/donately-openapi.yml
- filename: donately-openapi.yml
  format: yaml
  label: Donately Fundraisers API
  slug: donately-fundraisers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donately/refs/heads/main/openapi/donately-openapi.yml
- filename: donately-openapi.yml
  format: yaml
  label: Donately Subscriptions API
  slug: donately-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donately/refs/heads/main/openapi/donately-openapi.yml
- filename: donately-openapi.yml
  format: yaml
  label: Donately Accounts API
  slug: donately-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donately/refs/heads/main/openapi/donately-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Donately Authentication
name_suffix: Authentication
oauth_flows: []
overview: Donately secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Donately
provider_slug: donately
scheme_count: 1
schemes:
- description: HTTP Basic Auth. Use your Donately API token as the username with an empty password (the token is base64-encoded with a trailing colon). Find the token in the Donately dashboard under Settings -> API.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/donately-openapi.yml
  type: http
slug: donately-authentication
source_filename: donately-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/donately-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth. Use your Donately API token as the username with an empty password\n    (the token is base64-encoded with a trailing colon). Find the token in the Donately dashboard\n    under Settings -> API.\n  sources:\n  - openapi/donately-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/donately/refs/heads/main/authentication/donately-authentication.yml
summary_line: http · 1 scheme
tags:
- Fundraising
- Donations
- Nonprofit
- Payments
- Donor Management
- Recurring Giving
---
