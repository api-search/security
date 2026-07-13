---
api_key_in: []
api_specs:
- filename: linkedin-ads-openapi.yml
  format: yaml
  label: LinkedIn Marketing API
  slug: marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Linkedin Ads Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: LinkedIn Marketing API secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: LinkedIn Marketing API
provider_slug: linkedin-ads
scheme_count: 1
schemes:
- description: OAuth 2.0 three-legged (authorization code) flow.
  flows:
  - authorizationUrl: https://www.linkedin.com/oauth/v2/authorization
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: OAuth2
  sources:
  - openapi/linkedin-ads-openapi.yml
  type: oauth2
slug: linkedin-ads-authentication
source_filename: linkedin-ads-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/linkedin-ads-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.linkedin.com/oauth/v2/authorization\n    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n    scopes: 4\n  description: OAuth 2.0 three-legged (authorization code) flow.\n  sources:\n  - openapi/linkedin-ads-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/authentication/linkedin-ads-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Advertising
- Marketing
- LinkedIn
- Lead Generation
- Audience Targeting
- Conversions API
- Social Marketing
---
