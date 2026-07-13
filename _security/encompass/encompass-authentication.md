---
api_key_in: []
api_specs:
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Loan Management API
  slug: encompass-loan-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Loan Pipeline API
  slug: encompass-loan-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Borrower Pair & Applications API
  slug: encompass-borrower-pair-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Contacts API
  slug: encompass-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass eFolder Documents & Attachments API
  slug: encompass-efolder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Milestones & Associates API
  slug: encompass-milestones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Conditions API
  slug: encompass-conditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Users API
  slug: encompass-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Webhooks API
  slug: encompass-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Encompass Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Encompass secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Encompass
provider_slug: encompass
scheme_count: 2
schemes:
- description: OAuth 2.0 client credentials / authorization code issued per Encompass instance.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.elliemae.com/oauth2/v1/token
  name: oAuth2
  sources:
  - openapi/encompass-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/encompass-openapi.yml
  type: http
slug: encompass-authentication
source_filename: encompass-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/encompass-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.elliemae.com/oauth2/v1/token\n    scopes: 0\n  description: OAuth 2.0 client credentials / authorization code issued per Encompass instance.\n  sources:\n  - openapi/encompass-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/encompass-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/authentication/encompass-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Mortgage
- Loan Origination
- LOS
- Fintech
- ICE Mortgage Technology
- Ellie Mae
- Lending
---
