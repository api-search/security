---
api_key_in:
- query
api_specs:
- filename: trustpilot-business-units-openapi.yml
  format: yaml
  label: Trustpilot Business Units API
  slug: trustpilot-business-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/openapi/trustpilot-business-units-openapi.yml
- filename: trustpilot-service-reviews-openapi.yml
  format: yaml
  label: Trustpilot Service Reviews API
  slug: trustpilot-service-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/openapi/trustpilot-service-reviews-openapi.yml
- filename: trustpilot-invitation-openapi.yml
  format: yaml
  label: Trustpilot Invitation API
  slug: trustpilot-invitation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/openapi/trustpilot-invitation-openapi.yml
- filename: trustpilot-product-reviews-openapi.yml
  format: yaml
  label: Trustpilot Product Reviews API
  slug: trustpilot-product-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/openapi/trustpilot-product-reviews-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Trustpilot Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Trustpilot secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Trustpilot
provider_slug: trustpilot
scheme_count: 3
schemes:
- in: query
  name: ApiKey
  parameter: apikey
  sources:
  - openapi/trustpilot-business-units-openapi.yml
  - openapi/trustpilot-product-reviews-openapi.yml
  - openapi/trustpilot-service-reviews-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://authenticate.trustpilot.com/oauth/connect/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://authenticate.trustpilot.com/oauth/token
  name: OAuth2
  sources:
  - openapi/trustpilot-business-units-openapi.yml
  - openapi/trustpilot-product-reviews-openapi.yml
  - openapi/trustpilot-service-reviews-openapi.yml
  type: oauth2
- flows:
  - authorizationUrl: https://authenticate.trustpilot.com/oauth/connect/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://authenticate.trustpilot.com/oauth/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://authenticate.trustpilot.com/oauth/token
  name: OAuth2
  sources:
  - openapi/trustpilot-invitation-openapi.yml
  type: oauth2
slug: trustpilot-authentication
source_filename: trustpilot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trustpilot-business-units-openapi.yml, openapi/trustpilot-invitation-openapi.yml,\n  openapi/trustpilot-product-reviews-openapi.yml, openapi/trustpilot-service-reviews-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/trustpilot-business-units-openapi.yml\n  - openapi/trustpilot-product-reviews-openapi.yml\n  - openapi/trustpilot-service-reviews-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authenticate.trustpilot.com/oauth/connect/authorize\n    tokenUrl: https://authenticate.trustpilot.com/oauth/token\n    scopes: 1\n  sources:\n  - openapi/trustpilot-business-units-openapi.yml\n  - openapi/trustpilot-product-reviews-openapi.yml\n  - openapi/trustpilot-service-reviews-openapi.yml\n\
  - name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authenticate.trustpilot.com/oauth/connect/authorize\n    tokenUrl: https://authenticate.trustpilot.com/oauth/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://authenticate.trustpilot.com/oauth/token\n    scopes: 1\n  sources:\n  - openapi/trustpilot-invitation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/authentication/trustpilot-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Consumer Reviews
- Reviews
- Trust
- Ratings
- Business Profiles
- Product Reviews
---
