---
api_key_in: []
api_specs:
- filename: microsoft-linkedin-openapi.yml
  format: yaml
  label: LinkedIn Marketing API
  slug: marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/openapi/microsoft-linkedin-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Linkedin Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft LinkedIn secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft LinkedIn
provider_slug: microsoft-linkedin
scheme_count: 1
schemes:
- description: LinkedIn OAuth 2.0 (3-legged or 2-legged)
  flows:
  - authorizationUrl: https://www.linkedin.com/oauth/v2/authorization
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: oauth2
  sources:
  - openapi/microsoft-linkedin-openapi.yml
  type: oauth2
slug: microsoft-linkedin-authentication
source_filename: microsoft-linkedin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-linkedin-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.linkedin.com/oauth/v2/authorization\n    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n    scopes: 5\n  description: LinkedIn OAuth 2.0 (3-legged or 2-legged)\n  sources:\n  - openapi/microsoft-linkedin-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/authentication/microsoft-linkedin-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Marketing
- Microsoft
- Professional Networking
- Recruiting
- Social Network
---
