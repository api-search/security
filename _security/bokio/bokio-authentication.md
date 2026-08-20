---
api_key_in: []
api_specs:
- filename: bokio-authorization-api-openapi.yml
  format: yaml
  label: Bokio authorization API
  slug: bokio-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-authorization-api-openapi.yml
- filename: bokio-bank-payments-api-openapi.yml
  format: yaml
  label: Bokio bank-payments API
  slug: bokio-bank-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-bank-payments-api-openapi.yml
- filename: bokio-chart-of-accounts-api-openapi.yml
  format: yaml
  label: Bokio chart-of-accounts API
  slug: bokio-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-chart-of-accounts-api-openapi.yml
- filename: bokio-company-information-api-openapi.yml
  format: yaml
  label: Bokio company-information API
  slug: bokio-company-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-company-information-api-openapi.yml
- filename: bokio-connections-api-openapi.yml
  format: yaml
  label: Bokio connections API
  slug: bokio-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-connections-api-openapi.yml
- filename: bokio-credit-notes-api-openapi.yml
  format: yaml
  label: Bokio credit-notes API
  slug: bokio-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-credit-notes-api-openapi.yml
- filename: bokio-customers-api-openapi.yml
  format: yaml
  label: Bokio customers API
  slug: bokio-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-customers-api-openapi.yml
- filename: bokio-fiscal-years-api-openapi.yml
  format: yaml
  label: Bokio fiscal-years API
  slug: bokio-fiscal-years-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-fiscal-years-api-openapi.yml
- filename: bokio-invoices-api-openapi.yml
  format: yaml
  label: Bokio invoices API
  slug: bokio-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-invoices-api-openapi.yml
- filename: bokio-items-api-openapi.yml
  format: yaml
  label: Bokio items API
  slug: bokio-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-items-api-openapi.yml
- filename: bokio-journal-entries-api-openapi.yml
  format: yaml
  label: Bokio journal-entries API
  slug: bokio-journal-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-journal-entries-api-openapi.yml
- filename: bokio-sie-files-api-openapi.yml
  format: yaml
  label: Bokio sie-files API
  slug: bokio-sie-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-sie-files-api-openapi.yml
- filename: bokio-supplier-invoices-api-openapi.yml
  format: yaml
  label: Bokio supplier-invoices API
  slug: bokio-supplier-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-supplier-invoices-api-openapi.yml
- filename: bokio-suppliers-api-openapi.yml
  format: yaml
  label: Bokio suppliers API
  slug: bokio-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-suppliers-api-openapi.yml
- filename: bokio-tag-groups-api-openapi.yml
  format: yaml
  label: Bokio tag-groups API
  slug: bokio-tag-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-tag-groups-api-openapi.yml
- filename: bokio-uploads-api-openapi.yml
  format: yaml
  label: Bokio uploads API
  slug: bokio-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-uploads-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bokio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Bokio secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Bokio
provider_slug: bokio
scheme_count: 3
schemes:
- name: tokenAuth
  scheme: bearer
  sources:
  - openapi/bokio-company-api-openapi.yml
  - openapi/bokio-general-api-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /token
  - authorizationUrl: /authorize
    flow: authorizationCode
    scopes: 24
    tokenUrl: /token
  name: access_token
  sources:
  - openapi/bokio-company-api-openapi.yml
  - openapi/bokio-general-api-openapi.yml
  type: oauth2
- name: client_auth
  scheme: basic
  sources:
  - openapi/bokio-company-api-openapi.yml
  - openapi/bokio-general-api-openapi.yml
  type: http
slug: bokio-authentication
source_filename: bokio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/bokio-company-api-openapi.yml, openapi/bokio-general-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: tokenAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n  - openapi/bokio-general-api-openapi.yml\n- name: access_token\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /token\n    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: /authorize\n    tokenUrl: /token\n    scopes: 24\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n  - openapi/bokio-general-api-openapi.yml\n- name: client_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n  - openapi/bokio-general-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/authentication/bokio-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Fintech
- Accounting
- Bookkeeping
- Invoicing
- Payments
- Sweden
- SMB
- Authentication
---
