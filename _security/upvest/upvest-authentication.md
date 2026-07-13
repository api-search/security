---
api_key_in: []
api_specs:
- filename: upvest-investment-api-openapi.yml
  format: yaml
  label: Upvest Investment API
  slug: investment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upvest/refs/heads/main/openapi/upvest-investment-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Upvest Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Upvest secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Upvest
provider_slug: upvest
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials flow. Obtain an access token by providing your client ID and client secret.
  flows:
  - flow: clientCredentials
    scopes: 18
    tokenUrl: /auth/token
  name: oauth2ClientCredentials
  sources:
  - openapi/upvest-investment-api-openapi.yml
  type: oauth2
slug: upvest-authentication
source_filename: upvest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/upvest-investment-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n    scopes: 18\n  description: OAuth 2.0 client credentials flow. Obtain an access token by providing your client\n    ID and client secret.\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upvest/refs/heads/main/authentication/upvest-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Banking Infrastructure
- Fintech
- Investments
- Securities
- Fractional Investing
- Custody
- Wealth Management
---
