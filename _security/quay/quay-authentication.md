---
api_key_in: []
api_specs:
- filename: quay-openapi.yml
  format: yaml
  label: Quay
  slug: quay
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/openapi/quay-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Quay Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Quay secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Quay
provider_slug: quay
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://quay.io/oauth/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://quay.io/oauth/access_token
  name: OAuth2
  sources:
  - openapi/quay-openapi.yml
  type: oauth2
slug: quay-authentication
source_filename: quay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quay-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://quay.io/oauth/authorize\n    tokenUrl: https://quay.io/oauth/access_token\n    scopes: 6\n  sources:\n  - openapi/quay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/authentication/quay-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Container Images
- Containers
- Red Hat
- Registry
- Security Scanning
---
