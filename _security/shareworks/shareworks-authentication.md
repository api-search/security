---
api_key_in: []
api_specs:
- filename: postman.yaml
  format: yaml
  label: Shareworks Public API
  slug: shareworks-public-api
  spec_type: Postman
  url: https://www.postman.com/
- filename: shareworks-authentication-token-api-openapi.yml
  format: yaml
  label: Shareworks Authentication Token API
  slug: shareworks-authentication-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-authentication-token-api-openapi.yml
- filename: shareworks-authorized-capital-api-openapi.yml
  format: yaml
  label: Shareworks Authorized Capital API
  slug: shareworks-authorized-capital-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-authorized-capital-api-openapi.yml
- filename: shareworks-award-type-api-openapi.yml
  format: yaml
  label: Shareworks Award Type API
  slug: shareworks-award-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-award-type-api-openapi.yml
- filename: shareworks-company-api-openapi.yml
  format: yaml
  label: Shareworks Company API
  slug: shareworks-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-company-api-openapi.yml
- filename: shareworks-company-board-api-openapi.yml
  format: yaml
  label: Shareworks Company Board API
  slug: shareworks-company-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-company-board-api-openapi.yml
- filename: shareworks-company-integration-api-openapi.yml
  format: yaml
  label: Shareworks Company Integration API
  slug: shareworks-company-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-company-integration-api-openapi.yml
- filename: shareworks-entity-stakeholder-api-openapi.yml
  format: yaml
  label: Shareworks Entity Stakeholder API
  slug: shareworks-entity-stakeholder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-entity-stakeholder-api-openapi.yml
- filename: shareworks-grant-api-openapi.yml
  format: yaml
  label: Shareworks Grant API
  slug: shareworks-grant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-grant-api-openapi.yml
- filename: shareworks-holdings-api-openapi.yml
  format: yaml
  label: Shareworks Holdings API
  slug: shareworks-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-holdings-api-openapi.yml
- filename: shareworks-individual-stakeholder-api-openapi.yml
  format: yaml
  label: Shareworks Individual Stakeholder API
  slug: shareworks-individual-stakeholder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-individual-stakeholder-api-openapi.yml
- filename: shareworks-plan-api-openapi.yml
  format: yaml
  label: Shareworks Plan API
  slug: shareworks-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-plan-api-openapi.yml
- filename: shareworks-read-access-api-openapi.yml
  format: yaml
  label: Shareworks Read Access API
  slug: shareworks-read-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-read-access-api-openapi.yml
- filename: shareworks-stock-certificate-api-openapi.yml
  format: yaml
  label: Shareworks Stock Certificate API
  slug: shareworks-stock-certificate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-stock-certificate-api-openapi.yml
- filename: shareworks-stock-filing-api-openapi.yml
  format: yaml
  label: Shareworks Stock Filing API
  slug: shareworks-stock-filing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-stock-filing-api-openapi.yml
- filename: shareworks-vesting-schedule-api-openapi.yml
  format: yaml
  label: Shareworks Vesting Schedule API
  slug: shareworks-vesting-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-vesting-schedule-api-openapi.yml
- filename: shareworks-write-access-api-openapi.yml
  format: yaml
  label: Shareworks Write Access API
  slug: shareworks-write-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-write-access-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shareworks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shareworks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shareworks
provider_slug: shareworks
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: accessToken
  scheme: bearer
  sources:
  - openapi/shareworks-shareworks-public-api-openapi.yml
  type: http
slug: shareworks-authentication
source_filename: shareworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shareworks-shareworks-public-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/shareworks-shareworks-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/authentication/shareworks-authentication.yml
summary_line: http · 1 scheme
tags:
- Equity Compensation
- Stock Options
- RSU
- ESPP
- Employee Equity
- Financial-Services
- Morgan Stanley
- Equity Administration
- Private Companies
- Public Companies
---
