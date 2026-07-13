---
api_key_in: []
api_specs:
- filename: hmrc-vat-mtd-openapi.yml
  format: yaml
  label: HMRC VAT (Making Tax Digital) API
  slug: hmrc-vat-mtd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hmrc/refs/heads/main/openapi/hmrc-vat-mtd-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Hmrc Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: HMRC UK Tax Authority secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: HMRC UK Tax Authority
provider_slug: hmrc
scheme_count: 1
schemes:
- description: HMRC OAuth 2.0 Authorization Code grant (user-restricted)
  flows:
  - authorizationUrl: https://api.service.hmrc.gov.uk/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.service.hmrc.gov.uk/oauth/token
  name: OAuth2UserRestricted
  sources:
  - openapi/hmrc-vat-mtd-openapi.yml
  type: oauth2
slug: hmrc-authentication
source_filename: hmrc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hmrc-vat-mtd-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2UserRestricted\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.service.hmrc.gov.uk/oauth/authorize\n    tokenUrl: https://api.service.hmrc.gov.uk/oauth/token\n    scopes: 2\n  description: HMRC OAuth 2.0 Authorization Code grant (user-restricted)\n  sources:\n  - openapi/hmrc-vat-mtd-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hmrc/refs/heads/main/authentication/hmrc-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Government
- Making Tax Digital
- Regulatory
- Tax
- UK
---
