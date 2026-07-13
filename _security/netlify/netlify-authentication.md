---
api_key_in: []
api_specs:
- filename: netlify-openapi-original.yml
  format: yaml
  label: Netlify API
  slug: netlify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netlify/refs/heads/main/openapi/netlify-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Netlify Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Netlify secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Netlify
provider_slug: netlify
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://app.netlify.com/authorize
    flow: implicit
    scopes: 0
  name: netlifyAuth
  sources:
  - openapi/netlify-openapi-original.yml
  type: oauth2
slug: netlify-authentication
source_filename: netlify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/netlify-openapi-original.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: netlifyAuth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://app.netlify.com/authorize\n    scopes: 0\n  sources:\n  - openapi/netlify-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netlify/refs/heads/main/authentication/netlify-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- CDN
- Cloud
- Continuous Deployment
- Edge Computing
- JAMstack
- Serverless
- Serverless Functions
- Static Sites
- Web Hosting
- Websites
---
