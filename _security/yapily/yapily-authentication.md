---
api_key_in: []
api_specs:
- filename: yapily-platform-api-openapi.yml
  format: yaml
  label: Yapily Platform API
  slug: yapily-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-platform-api-openapi.yml
- filename: yapily-institutions-api-openapi.yml
  format: yaml
  label: Yapily Institutions API
  slug: yapily-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-institutions-api-openapi.yml
- filename: yapily-consents-api-openapi.yml
  format: yaml
  label: Yapily Consents and Authorisations API
  slug: yapily-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-consents-api-openapi.yml
- filename: yapily-data-api-openapi.yml
  format: yaml
  label: Yapily Data Access API (AIS)
  slug: yapily-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-data-api-openapi.yml
- filename: yapily-payments-api-openapi.yml
  format: yaml
  label: Yapily Payments API (PIS)
  slug: yapily-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-payments-api-openapi.yml
- filename: yapily-vrp-api-openapi.yml
  format: yaml
  label: Yapily Variable Recurring Payments API
  slug: yapily-vrp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-vrp-api-openapi.yml
- filename: yapily-hosted-pages-api-openapi.yml
  format: yaml
  label: Yapily Hosted Pages API
  slug: yapily-hosted-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-hosted-pages-api-openapi.yml
- filename: yapily-data-plus-api-openapi.yml
  format: yaml
  label: Yapily Data Plus API
  slug: yapily-data-plus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-data-plus-api-openapi.yml
- filename: yapily-beneficiaries-api-openapi.yml
  format: yaml
  label: Yapily Beneficiaries API
  slug: yapily-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-beneficiaries-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Yapily Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yapily secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Yapily
provider_slug: yapily
scheme_count: 1
schemes:
- description: Use HTTP Basic Authentication with your Application ID as username and Application Secret as password. Manage credentials in the [Yapily Console](https://console.yapily.com/). See [Authentication](/api-reference/authentication) for details.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/yapily-beneficiaries-api-openapi.yml
  - openapi/yapily-consents-api-openapi.yml
  - openapi/yapily-data-api-openapi.yml
  - openapi/yapily-data-plus-api-openapi.yml
  - openapi/yapily-hosted-pages-api-openapi.yml
  - openapi/yapily-institutions-api-openapi.yml
  - openapi/yapily-payments-api-openapi.yml
  - openapi/yapily-platform-api-openapi.yml
  - openapi/yapily-vrp-api-openapi.yml
  type: http
slug: yapily-authentication
source_filename: yapily-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/yapily-beneficiaries-api-openapi.yml, openapi/yapily-consents-api-openapi.yml,\n  openapi/yapily-data-api-openapi.yml, openapi/yapily-data-plus-api-openapi.yml, openapi/yapily-hosted-pages-api-openapi.yml,\n  openapi/yapily-institutions-api-openapi.yml, openapi/yapily-payments-api-openapi.yml, openapi/yapily-platform-api-openapi.yml,\n  openapi/yapily-vrp-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Use HTTP Basic Authentication with your Application ID as username and Application\n    Secret as password. Manage credentials in the [Yapily Console](https://console.yapily.com/).\n    See [Authentication](/api-reference/authentication) for details.\n  sources:\n  - openapi/yapily-beneficiaries-api-openapi.yml\n  - openapi/yapily-consents-api-openapi.yml\n  - openapi/yapily-data-api-openapi.yml\n  - openapi/yapily-data-plus-api-openapi.yml\n  -\
  \ openapi/yapily-hosted-pages-api-openapi.yml\n  - openapi/yapily-institutions-api-openapi.yml\n  - openapi/yapily-payments-api-openapi.yml\n  - openapi/yapily-platform-api-openapi.yml\n  - openapi/yapily-vrp-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/authentication/yapily-authentication.yml
summary_line: http · 1 scheme
tags:
- Open Banking
- AISP
- PISP
- Payments
- Account Information
- Variable Recurring Payments
- Financial Services
- PSD2
- FCA
- Berlin Group
- UK
- Europe
- FinTech
---
