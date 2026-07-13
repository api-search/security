---
api_key_in: []
api_specs:
- filename: webflow-data-api-openapi.yml
  format: yaml
  label: Webflow Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow-api-and-documentation-webflow/refs/heads/main/openapi/webflow-data-api-openapi.yml
- filename: webflow-sites-openapi.yml
  format: yaml
  label: Webflow Sites API
  slug: sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow-api-and-documentation-webflow/refs/heads/main/openapi/webflow-sites-openapi.yml
- filename: webflow-collections-openapi.yml
  format: yaml
  label: Webflow Collections API
  slug: collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow-api-and-documentation-webflow/refs/heads/main/openapi/webflow-collections-openapi.yml
- filename: webflow-items-openapi.yml
  format: yaml
  label: Webflow CMS Items API
  slug: items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow-api-and-documentation-webflow/refs/heads/main/openapi/webflow-items-openapi.yml
- filename: webflow-webhooks-openapi.yml
  format: yaml
  label: Webflow Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow-api-and-documentation-webflow/refs/heads/main/openapi/webflow-webhooks-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Webflow Api And Documentation Webflow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Webflow API and Documentation secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Webflow API and Documentation
provider_slug: webflow-api-and-documentation-webflow
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://webflow.com/oauth/authorize
    flow: authorizationCode
    scopes: 26
    tokenUrl: https://api.webflow.com/oauth/token
  name: OAuth2
  sources:
  - openapi/webflow-collections-openapi.yml
  - openapi/webflow-data-api-openapi.yml
  - openapi/webflow-items-openapi.yml
  - openapi/webflow-sites-openapi.yml
  - openapi/webflow-webhooks-openapi.yml
  type: oauth2
- name: ApiKey
  scheme: bearer
  sources:
  - openapi/webflow-collections-openapi.yml
  - openapi/webflow-data-api-openapi.yml
  - openapi/webflow-items-openapi.yml
  - openapi/webflow-sites-openapi.yml
  - openapi/webflow-webhooks-openapi.yml
  type: http
slug: webflow-api-and-documentation-webflow-authentication
source_filename: webflow-api-and-documentation-webflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/webflow-collections-openapi.yml, openapi/webflow-data-api-openapi.yml, openapi/webflow-items-openapi.yml,\n  openapi/webflow-sites-openapi.yml, openapi/webflow-webhooks-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://webflow.com/oauth/authorize\n    tokenUrl: https://api.webflow.com/oauth/token\n    scopes: 26\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- name: ApiKey\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webflow-api-and-documentation-webflow/refs/heads/main/authentication/webflow-api-and-documentation-webflow-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- CMS
- Content Management
- Ecommerce
- No-Code
- Publishing
- Web Development
---
