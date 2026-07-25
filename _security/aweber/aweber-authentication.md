---
api_key_in: []
api_specs:
- filename: aweber-accounts-api-openapi.yml
  format: yaml
  label: AWeber Accounts API
  slug: aweber-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-accounts-api-openapi.yml
- filename: aweber-broadcasts-api-openapi.yml
  format: yaml
  label: AWeber Broadcasts API
  slug: aweber-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-broadcasts-api-openapi.yml
- filename: aweber-campaigns-api-openapi.yml
  format: yaml
  label: AWeber Campaigns API
  slug: aweber-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-campaigns-api-openapi.yml
- filename: aweber-custom-fields-api-openapi.yml
  format: yaml
  label: AWeber Custom Fields API
  slug: aweber-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-custom-fields-api-openapi.yml
- filename: aweber-landing-pages-api-openapi.yml
  format: yaml
  label: AWeber Landing Pages API
  slug: aweber-landing-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-landing-pages-api-openapi.yml
- filename: aweber-lists-api-openapi.yml
  format: yaml
  label: AWeber Lists API
  slug: aweber-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-lists-api-openapi.yml
- filename: aweber-segments-api-openapi.yml
  format: yaml
  label: AWeber Segments API
  slug: aweber-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-segments-api-openapi.yml
- filename: aweber-subscribers-api-openapi.yml
  format: yaml
  label: AWeber Subscribers API
  slug: aweber-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-subscribers-api-openapi.yml
- filename: aweber-web-forms-api-openapi.yml
  format: yaml
  label: AWeber Web Forms API
  slug: aweber-web-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-web-forms-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Aweber Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AWeber secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AWeber
provider_slug: aweber
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://auth.aweber.com/oauth2/authorize
    flow: authorizationCode
    scopes: 9
    tokenUrl: https://auth.aweber.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/aweber-openapi.yml
  type: oauth2
slug: aweber-authentication
source_filename: aweber-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aweber-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.aweber.com/oauth2/authorize\n    tokenUrl: https://auth.aweber.com/oauth2/token\n    scopes: 9\n  sources:\n  - openapi/aweber-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/authentication/aweber-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Email Marketing
- Marketing Automation
- Email
- Newsletters
- Subscribers
- Campaigns
- Landing Pages
---
