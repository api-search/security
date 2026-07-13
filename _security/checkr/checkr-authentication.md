---
api_key_in: []
api_specs:
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Candidates API
  slug: checkr-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Invitations API
  slug: checkr-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Reports API
  slug: checkr-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Screenings API
  slug: checkr-screenings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Verifications API
  slug: checkr-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Packages API
  slug: checkr-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Documents API
  slug: checkr-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Adverse Actions API
  slug: checkr-adverse-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Subscriptions API
  slug: checkr-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Continuous Checks API
  slug: checkr-continuous-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Nodes and Hierarchy API
  slug: checkr-nodes-hierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Geos API
  slug: checkr-geos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Webhooks API
  slug: checkr-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Checkr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Checkr secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Checkr
provider_slug: checkr
scheme_count: 1
schemes:
- description: HTTP Basic auth with your secret API key as the username and an empty password. Checkr Partner integrations authenticate on behalf of customer accounts using OAuth instead.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/checkr-openapi.yml
  type: http
slug: checkr-authentication
source_filename: checkr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/checkr-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth with your secret API key as the username and an empty password.\n    Checkr Partner integrations authenticate on behalf of customer accounts using OAuth instead.\n  sources:\n  - openapi/checkr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/authentication/checkr-authentication.yml
summary_line: http · 1 scheme
tags:
- Background Checks
- Employment Screening
- Compliance
- HR Tech
- Identity Verification
- Criminal Records
---
