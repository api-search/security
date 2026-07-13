---
api_key_in: []
api_specs:
- filename: generate-a-client-from-openapi-definition
  format: yaml
  label: Moody's KYC API
  slug: moodys
  spec_type: OpenAPI
  url: 'https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/

    https://www.kompany.com/kycapi/docs/resources/resources/customer-facing-documents/generate-a-client-from-openapi-definition'
- filename: moodys-data-buffet-api-openapi.yml
  format: yaml
  label: Moody's Data Buffet API
  slug: data-buffet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-data-buffet-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Moodys Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Moody's secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Moody's
provider_slug: moodys
scheme_count: 1
schemes:
- description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id and client_secret from your Moody's Analytics account.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.economy.com/data/v1/oauth2/token
  name: oauth2
  sources:
  - openapi/moodys-data-buffet-api-openapi.yml
  type: oauth2
slug: moodys-authentication
source_filename: moodys-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moodys-data-buffet-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/data/v1/oauth2/token\n    scopes: 0\n  description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id\n    and client_secret from your Moody's Analytics account.\n  sources:\n  - openapi/moodys-data-buffet-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/authentication/moodys-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Climate Risk
- Compliance
- Credit Risk
- Economic Data
- Entity Verification
- Financial Analytics
- Insurance
- KYC
- Risk
- Screening
---
