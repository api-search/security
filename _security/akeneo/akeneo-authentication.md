---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Akeneo PIM REST API
  slug: pim-rest-api
  spec_type: OpenAPI
  url: https://storage.googleapis.com/akecld-prd-pim-saas-shared-openapi-spec/openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Akeneo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Akeneo secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Akeneo
provider_slug: akeneo
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{tenant}.cloud.akeneo.com/api/oauth/v1/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/akeneo-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/akeneo-openapi.yml
  type: http
slug: akeneo-authentication
source_filename: akeneo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/akeneo-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.cloud.akeneo.com/api/oauth/v1/token\n    scopes: 0\n  sources:\n  - openapi/akeneo-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/akeneo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/authentication/akeneo-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Product Information Management
- PIM
- Product Data
- Catalog Management
- Commerce
- Retail
---
