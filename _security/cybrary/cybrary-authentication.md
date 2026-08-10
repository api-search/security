---
api_key_in: []
api_specs:
- filename: cybrary-completions-api-openapi.yml
  format: yaml
  label: Cybrary Completions API
  slug: cybrary-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybrary/refs/heads/main/openapi/cybrary-completions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cybrary Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cybrary secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cybrary
provider_slug: cybrary
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials. Credentials are issued by Cybrary to the customer organization; client authentication is sent as a HTTP Basic Authorization header.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://app.cybrary.it/auth/oauth/token
  name: oauth2
  sources:
  - openapi/cybrary-completions-export-openapi.yml
  type: oauth2
slug: cybrary-authentication
source_filename: cybrary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://help.cybrary.it/completions-export-integration\ndocs: https://help.cybrary.it/completions-export-integration\nderived_from: openapi/cybrary-completions-export-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.cybrary.it/auth/oauth/token\n    scopes: 1\n  description: OAuth 2.0 client credentials. Credentials are issued by Cybrary to the customer\n    organization; client authentication is sent as a HTTP Basic Authorization header.\n  sources:\n  - openapi/cybrary-completions-export-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybrary/refs/heads/main/authentication/cybrary-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Cybersecurity
- Training
- Education
- Learning Management
- Certification
- Workforce Development
- xAPI
- SCIM
- Security Awareness
---
