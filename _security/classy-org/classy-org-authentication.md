---
api_key_in: []
api_specs:
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Organizations API
  slug: classy-org-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Campaigns API
  slug: classy-org-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Fundraising Pages API
  slug: classy-org-fundraising-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Fundraising Teams API
  slug: classy-org-fundraising-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Transactions API
  slug: classy-org-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Recurring Donation Plans API
  slug: classy-org-recurring-donation-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Members API
  slug: classy-org-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Supporters API
  slug: classy-org-supporters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Designations API
  slug: classy-org-designations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Classy Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: Classy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Classy
provider_slug: classy-org
scheme_count: 1
schemes:
- description: 'OAuth2 client_credentials access token obtained from POST /oauth2/auth. Passed as `Authorization: Bearer {access_token}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/classy-org-openapi.yml
  type: http
slug: classy-org-authentication
source_filename: classy-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/classy-org-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth2 client_credentials access token obtained from POST /oauth2/auth. Passed\n    as `Authorization: Bearer {access_token}`.'\n  sources:\n  - openapi/classy-org-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/authentication/classy-org-authentication.yml
summary_line: http · 1 scheme
tags:
- Nonprofit
- Fundraising
- Donations
- Peer to Peer
- Philanthropy
- Payments
- GoFundMe Pro
---
