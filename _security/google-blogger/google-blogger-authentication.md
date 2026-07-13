---
api_key_in:
- query
api_specs:
- filename: blogger.yml
  format: yaml
  label: Google Blogger API V3
  slug: google-blogger
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-blogger/refs/heads/main/openapi/blogger.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Blogger Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Blogger secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Blogger
provider_slug: google-blogger
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/blogger.yml
  type: oauth2
- in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/blogger.yml
  type: apiKey
slug: google-blogger-authentication
source_filename: google-blogger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blogger.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/blogger.yml\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/blogger.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-blogger/refs/heads/main/authentication/google-blogger-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Blogging
- CMS
- Comments
- Google
- Pages
- Posts
- Publishing
---
