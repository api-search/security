---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Dropbox Sign REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://github.com/hellosign/hellosign-openapi/blob/main/openapi.yaml
- filename: dropbox-sign-events-asyncapi.yml
  format: yaml
  label: Dropbox Sign Events and Callbacks API
  slug: events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/dropbox-sign/refs/heads/main/asyncapi/dropbox-sign-events-asyncapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Dropbox Sign Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Dropbox Sign secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Dropbox Sign
provider_slug: dropbox-sign
scheme_count: 2
schemes:
- description: Dropbox Sign API key used as Basic auth username with empty password
  name: apiKey
  scheme: basic
  sources:
  - openapi/dropbox-sign-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://app.hellosign.com/oauth/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://app.hellosign.com/oauth/token
  name: oauth2
  sources:
  - openapi/dropbox-sign-openapi.yml
  type: oauth2
slug: dropbox-sign-authentication
source_filename: dropbox-sign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dropbox-sign-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: http\n  scheme: basic\n  description: Dropbox Sign API key used as Basic auth username with empty password\n  sources:\n  - openapi/dropbox-sign-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.hellosign.com/oauth/authorize\n    tokenUrl: https://app.hellosign.com/oauth/token\n    scopes: 5\n  sources:\n  - openapi/dropbox-sign-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dropbox-sign/refs/heads/main/authentication/dropbox-sign-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- eSignature
- Electronic Signature
- Document Signing
- Workflow Automation
- Documents
---
