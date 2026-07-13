---
api_key_in: []
api_specs:
- filename: dns-openapi.yml
  format: yaml
  label: Google Cloud DNS API
  slug: google-cloud-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dns/refs/heads/main/openapi/dns-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Cloud Dns Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud DNS secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud DNS
provider_slug: google-cloud-dns
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/dns-openapi.yml
  type: oauth2
slug: google-cloud-dns-authentication
source_filename: google-cloud-dns-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dns-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/dns-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dns/refs/heads/main/authentication/google-cloud-dns-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- DNS
- Domain Names
- Google Cloud
- Name Resolution
- Networking
---
